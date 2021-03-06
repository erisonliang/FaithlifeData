# Version History

### 1.0.0

* Official release.

### 0.300.1

* Try to avoid assembly binding errors from downstream dependencies.

### 0.300.0

* **Breaking:** Allow `object` to return a single field as-is instead of building a dynamic object with one property.
* **Breaking:** Make `ProviderMethods` property internal (otherwise it seems important to the API).
* **Breaking:** Use `ValueTask` instead of `Task`.
* **Breaking:** Rename `read` parameter to `map`.
* Ignore underscores when mapping fields to DTO properties.
* Support index/range and `IAsyncEnumerable` on .NET Standard 2.0.
* Support `IAsyncDisposable`.
* Add `Enumerate` to `DbConnectorResultSets`.
* Support mapping records to dictionaries.
* Add null record fields when mapping to dynamic.

### 0.200.0

* **Breaking:** Eliminate `DataRecordUtility`.
* **Breaking:** Rename `DbConnectorResultSet` to `DbConnectorResultSets`.
* **Breaking:** Make `DbParameters` an immutable `struct`.
* **Breaking:** Use `count` parameter name consistently.
* **Breaking:** Support nullable reference types. Make some previously nullable parameters and properties non-nullable.
* Add `QueryMultipleAsync`.
* Add `EnumerateAsync`, which uses the new `IAsyncEnumerable` (.NET Standard 2.1).
* Support index/range for data record access (.NET Standard 2.1).
* Expose text and parameters of commands.
* Support new async ADO.NET methods from .NET Standard 2.1.
* Add XML documentation comments.
* Improve NuGet package description and tags.

### 0.100.1

* Fix bug with QueryFirst/Single and multiple result sets.

### 0.100.0

* Advance version past internal version.

### 0.10.0

* Stop using CommandBehavior.SequentialAccess.

### 0.1.0

* Initial release.
