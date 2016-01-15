# TypeScript Debugging

1. Add a tsconfig.json file and configure it.

    ```json
    {
        "compilerOptions": {
            "target": "es5",
            "module": "commonjs",
            "sourceMap": true
        }
    }
    ```

2. Create tasks.json

  - Type Shift+Cmd+P, type `config`, then select Configure Task Runner
  - A tasks.json file will be added to the .vscode folder
  
3. Add a file called HelloWorld.ts, then paste the following:

    ```typescript
    class Startup {
        public static main(): number {
            console.log("Hello World");
            return 0;
        }
    }
    ```
    
4. Press Cmd+B to compile the TypeScript into ES5 JavaScript.

  - A HelloWorld.js file should appear