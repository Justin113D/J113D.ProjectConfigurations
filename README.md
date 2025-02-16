# J113D Project Configuration

This repository hosts reused project configurations for all J113D projects.
<br/> (Greatly inspired by the [Reloaded Project](https://github.com/Reloaded-Project/Reloaded.Project.Configurations))

This includes:

- `.editorconfig` files for configuring code style.
- `NuGet.Build.props` for common project settings that target NuGet.
- `Directory.Build.props` for common project settings.

## Usage

To use this repository, add it as a submodule to your project.

```
git submodule add https://github.com/Justin113D/J113D.ProjectConfigurations.git ./src/J113D.ProjectConfigurations
```

Periodically update the submodule to the latest version.

```
git submodule update --remote
```

## Code Style

The code style is defined in the `.editorconfig` file in the root of the repo.

To apply this to your project, do the following:

- Enable symlinks for your git installation by running `git config core.symlinks true`.
- Make symlink to `J113D.ProjectConfigurations/.editorconfig` in the root of your project.
- In cmd you can do `mklink .editorconfig J113D.ProjectConfigurations\.editorconfig` as admin.
- Or on Linux, you can do `ln -s "J113D.ProjectConfigurations/.editorconfig" ".editorconfig"`.

## File Layout

The following is the expected file layout for your project:

```
- docs/
- src/
```

The `docs` folder should contain all documentation for your project (if present).
The `src` folder should contain all source code for your project.

## License

This repository is licensed under the GPLv3 license; as per the license of J113D.
