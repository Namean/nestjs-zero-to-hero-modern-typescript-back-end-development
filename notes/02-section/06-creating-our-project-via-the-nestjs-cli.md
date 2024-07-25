# Section 2: Task Management Application (REST API)
## 6. Creating our project via the NestJS CLI

```bash
$ nest new nestjs-task-management
```
```
```

- nest new nestjs-task-management
- Select yarn as the package manager


## If [ nest not found after installing with yarn 
     ```bash
     export PATH="$PATH:$(yarn global bin)"
     ```

     Then, reload your shell configuration:
]

If you've installed the `nest` CLI tool using `yarn` and are encountering a "command not found" error, it could be due to several reasons. Here’s how you can troubleshoot and resolve the issue:

1. **Check Installation**
     ```bash
     source ~/.bashrc  # or source ~/.zshrc
     ```

: Ensure that `nest` is properly installed. Run:

   ```bash
   yarn global list

   ```bash
   nest --version

4. **Reinstall**: Sometimes reinstalling can resolve path or installation issues. Uninstall and then reinstall `@nestjs/cli`:
If none of these solutions work, there might be a specific issue with your environment or configuration. Let me know if you need further help!
   ```bash
   npx @nestjs/cli new project-name
   ```


5. **Use `npx`**: As an alternative, you can use `npx` to run the `nest` CLI without installing it globally:
   yarn global remove @nestjs/cli
   yarn global add @nestjs/cli
   ```

   ```bash
   ```

   If it still doesn’t work, there may have been an issue during installation.
   - **Windows**: Global binaries are typically installed in `%LOCALAPPDATA%\Yarn\bin`. Ensure this directory is in your system `PATH`.

3. **Verify Installation**: Check if the `nest` command is available:
   ```

   Look for `@nestjs/cli` in the list. If it's not there, you might need to install it globally:

   ```bash
   yarn global add @nestjs/cli
   ```

2. **Verify Path**: Make sure the global `yarn` binaries are in your system’s `PATH`. The location depends on your operating system and how Yarn is configured.

   - **Linux/MacOS**: Usually, Yarn installs global binaries in `~/.yarn/bin`. You can add this to your `PATH` by adding the following line to your `.bashrc`, `.zshrc`, or equivalent shell configuration file:

