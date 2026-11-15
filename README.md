# cloudpkg-recipes

Collection of 25,000 package recipes for CloudOS Package Manager (cloudpkg).

## Format

Each package has:
- `{package}-{version}.cpr` - Recipe file in CPR format
- `Manifest` - Checksum file

## Structure

Recipes are organized in categories:
- system/ (apps, libs, utils, etc.)
- net/ (http, ftp, dns, etc.)
- media/ (gfx, sound, video, etc.)
- games/ (action, arcade, strategy, etc.)
- dev/ (lang, libs, tools, etc.)
- And more...

## Usage

Add this repository to your cloudpkg configuration:
```bash
# Add to cloudpkg repos
cloudpkg repo add cloudpkg-recipes https://github.com/wh1laye/cloudpkg-recipes.git

# Or use local path
cloudpkg repo add cloudpkg-recipes /path/to/cloudpkg-recipes

# Sync and install
cloudpkg sync
cloudpkg install <package>
```

## License

All recipes are distributed under the terms of the CloudOS License.
Independent implementation, not based on any other distribution.
