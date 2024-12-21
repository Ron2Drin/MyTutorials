# Run C project

1. Copy the following and paste to terminal

```
mkdir [project_name]
cd project_name
code .
```

2. Create exactuables using run code on the right (`tasks.json` and more files are created)

3. Create the following `launch.json` inside .vscode

```
{
  "version": "0.2.0",
  "configurations": [
    {
      "type": "lldb",
      "request": "launch",
      "name": "Debug",
      "program": "${fileDirname}/${fileBasenameNoExtension}",
      "args": [],
      "cwd": "${fileDirname}"
    }
  ]
}
```
3. Run
