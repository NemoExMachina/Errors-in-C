# Errors-in-C
<html>
    <head>
        <title>Errors in C</title>
        <style>
            body {
                font-family: Arial, sans-serif;
                background-color: #f3f3f3;
                color: #333;
                margin: 0;
                padding: 0;
                line-height: 1.6;
            }
            .code-container {
                background-color: #282c34;
                color: #61dafb;
                padding: 16px;
                border-radius: 8px;
                font-family: Consolas, "Courier New", monospace;
            }
            .code-container span.keyword {
                color: #d19a66;
                font-weight: bold;
            }
            .code-container span.string {
                color: #98c379;
            }
            .code-container span.identifier {
                color: #61dafb;
            }
            .code-container span.constant {
                color: #d19a66;
            }
            .code-container span.operator {
                color: #c678dd;
            }
            .code-container span.special-symbol {
                color: #56b6c2;
            }
            .code-container span.error {
                color: #e06c75;
                font-weight: bold;
            }
        </style>
    </head>
    <body>
        <div class="code-container">
            <h2>Program demonstrating various types of errors in C</h2>
            <pre>
    #include<<span class="keyword">stdio</span>.h&gt;
    <span class="keyword">int</span><span class="function"> main</span>() {
        <span class="keyword">int</span> <span class="identifier">a</span> = <span class="constant">10</span>;
        <span class="keyword">int</span> <span class="identifier">b</span> = <span class="constant">0</span>;
        <span class="comment">// Syntax Error: Missing semicolon</span>
        <span class="identifier">printf</span>(<span class="string">"Hello, World!"</span>) <span class="error">// Error: expected ';' before '}' token</span>
        <span class="comment">// Semantic Error: Division by zero</span>
        <span class="keyword">int</span> <span class="identifier">c</span> = <span class="identifier">a</span> <span class="operator">/</span> <span class="identifier">b</span>; <span class="error">// Error: division by zero</span>
        <span class="comment">// Logical Error: Incorrect calculation</span>
        <span class="keyword">int</span> <span class="identifier">d</span> = <span class="identifier">a</span> <span class="operator">*</span> <span class="constant">2</span>; <span class="error">// Error: should be 'a + 2' instead of 'a * 2'</span>
        <span class="identifier">printf</span>(<span class="string">"Result: %d\n"</span>, <span class="identifier">d</span>);
        <span class="keyword">return</span> <span class="constant">0</span>;
    }
            </pre>
            <center>
            <img src="Errors.png" alt="Output" width="400" height="250">
            </center>
        </div>
    </body>
</html>
