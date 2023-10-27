# halogen

The script is to migrate repositories with `ghe-migrator` from a GitHub Enterprise instance to another instance.

### How to use

1. Set the *halogen.conf* some information.

   e.g)

   ```
   # SOURCE SETTINGS
   SOURCE_INSTANCE=source.host
   SOURCE_USER=pnsk
   SOURCE_TOKEN=token

   # TARGET SETTINGS
   TARGET_INSTANCE=target.host
   TARGET_USER=pnsk
   TARGET_TOKEN=token
   ```

2. Run the command with specifying repositories you want to migrate.

   ```
   ./halogen <org>/<repo>
   ```

   If you want to migrate multiple repositories, please add the repository with `,`:

   ```
   ./halogen <org1>/<repo1>,<org2>/<repo2>
   ```
