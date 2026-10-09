// 1. Initialize and run the parser on script source code const parser = new Parser(sourceCode, "script.js"); parser.parse();

// 2. Compile the parsed AST into bytecode routines const compiler = new Compiler(parser.program);

// 3. Instantiate an execution context and run the compiled program const context = { global: {}, warnings: { using_undefined_variable: {}, assigning_field_to_undefined: {}, invoking_non_function: {} } };

compiler.exec(context);
(https://raw.githubusercontent.com/SharKingStudios/Starbie/refs/heads/main/GuidePics/Starbie%20Render.png)
