# @lassehaslev/executor
> Run a command every time a file change. Its that simple.

## Install
```bash
# Install project globaly
npm install -g @lassehaslev/executor

# Install executor per project
npm install @lassehaslev/executor --save-dev
```

## Usage
### Command line
```bash
executor "<command>"
    [--run-on-first=true]
    [--watch="**/*"]
    [--ignore=""]
```

### Npm
package.json
```json
{
    "scripts": {
        "executor": "executor '<command>' [options]",
    }
}
```
Now you can run the command ```npm run executor``` from command line.

Path if you run per project and not in a npm script
```bash
./node_modules/.bin/executor
```

## Development
```bash
# link to local command line
npm link

# compile to es6
npm run dev

# When you are finished unlink local command
npm unlink
```