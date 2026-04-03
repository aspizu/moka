# Modules and Packages

Modules are files. Packages are directories. Packages don't have any files associated
with them, except for the root package.

Packages can only contain modules or other packages, packages cannot contain functions, etc.

Modules can only contain functions, etc.

## Library Imports

`PackageName` is a library package.

```moka
import PackageName
```

Sub-modules or sub-packages can be accessed using the dot notation: `PackageName.SubPackageName`, `PackageName.SubModuleName`.

### Import sub-packages or sub-modules into the current scope

`PackageName`contains the sub-package `SubPackageName`.

```moka
import PackageName.SubPackageName
```

`SubPackageName` is available in the current scope.

### Import functions, etc. from a module into the current scope

```moka
import PackageName.SubPackageName.SubModuleName.function_name
```

`function_name` is available in the current scope.

## Relative and project-absolute imports

### Import a module relative to the current package

```moka
import .ModuleName
```

### Import a module relative to the parent package of the current package

```moka
import ..ModuleName
```

### Import a module relative to the project root package

```moka
import root.ModuleName
```
