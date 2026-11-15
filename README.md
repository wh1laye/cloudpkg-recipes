# cloudpkg-recipes

Collection of package recipes for CloudOS package manager (cloudpkg).

## Format

Each package has:
- `{package}-{version}.cpr` - Recipe file
- `Manifest` - Checksum file

## Structure

Recipes are organized in categories (app-*, dev-*, net-*, sys-*, etc.)

## Usage

Copy to /var/db/repos/cloudpkg-recipes and sync:
```bash
ln -s /path/to/cloudpkg-recipes /var/db/repos/cloudpkg-recipes
cp /var/db/repos/cloudpkg-recipes/etc/portage/repos.conf/cloudpkg-recipes.conf /etc/portage/repos.conf/
emerge --sync
```
