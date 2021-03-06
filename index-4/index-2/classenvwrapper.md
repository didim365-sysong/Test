# class tensorflow::EnvWrapper

An implementation of Env that forwards all calls to another Env .

May be useful to clients who wish to override just part of the functionality of another Env .

## Member Details

### `tensorflow::EnvWrapper::EnvWrapper(Env *t)` <a id="tensorflow_EnvWrapper_EnvWrapper"></a>

Initializes an EnvWrapper that delegates all calls to \*t.

### `tensorflow::EnvWrapper::~EnvWrapper()` <a id="tensorflow_EnvWrapper_EnvWrapper"></a>

### `Env* tensorflow::EnvWrapper::target() const` <a id="Env_tensorflow_EnvWrapper_target"></a>

Returns the target to which this Env forwards all calls.

### `Status tensorflow::EnvWrapper::GetFileSystemForFile(const string &fname, FileSystem **result) override` <a id="Status_tensorflow_EnvWrapper_GetFileSystemForFile"></a>

Returns the FileSystem object to handle operations on the file specified by 'fname'. The FileSystem object is used as the implementation for the file system related \(non-virtual\) functions that follow. Returned FileSystem object is still owned by the Env object and will.

### `Status tensorflow::EnvWrapper::GetRegisteredFileSystemSchemes(std::vector< string > *schemes) override` <a id="Status_tensorflow_EnvWrapper_GetRegisteredFileSystemSchemes"></a>

Returns the file system schemes registered for this Env .

### `Status tensorflow::EnvWrapper::RegisterFileSystem(const string &scheme, FileSystemRegistry::Factory factory) override` <a id="Status_tensorflow_EnvWrapper_RegisterFileSystem"></a>

### `uint64 tensorflow::EnvWrapper::NowMicros() override` <a id="uint64_tensorflow_EnvWrapper_NowMicros"></a>

Returns the number of micro-seconds since some fixed point in time. Only useful for computing deltas of time.

### `void tensorflow::EnvWrapper::SleepForMicroseconds(int micros) override` <a id="void_tensorflow_EnvWrapper_SleepForMicroseconds"></a>

Sleeps/delays the thread for the prescribed number of micro-seconds.

### `Thread* tensorflow::EnvWrapper::StartThread(const ThreadOptions &thread_options, const string &name, std::function< void()> fn) override` <a id="Thread_tensorflow_EnvWrapper_StartThread"></a>

Returns a new thread that is running fn\(\) and is identified \(for debugging/performance-analysis\) by "name".

Caller takes ownership of the result and must delete it eventually \(the deletion will block until fn\(\) stops running\).

### `void tensorflow::EnvWrapper::SchedClosure(std::function< void()> closure) override` <a id="void_tensorflow_EnvWrapper_SchedClosure"></a>

### `void tensorflow::EnvWrapper::SchedClosureAfter(int micros, std::function< void()> closure) override` <a id="void_tensorflow_EnvWrapper_SchedClosureAfter"></a>

### `Status tensorflow::EnvWrapper::LoadLibrary(const char *library_filename, void **handle) override` <a id="Status_tensorflow_EnvWrapper_LoadLibrary"></a>

### `Status tensorflow::EnvWrapper::GetSymbolFromLibrary(void *handle, const char *symbol_name, void **symbol) override` <a id="Status_tensorflow_EnvWrapper_GetSymbolFromLibrary"></a>

