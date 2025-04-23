<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>LaunchPad | Powered by ProDevStudio</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.16/dist/tailwind.min.css" rel="stylesheet">
  <script src="https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.34.1/min/vs/loader.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/FileSaver.js/2.0.5/FileSaver.min.js"></script>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background-color: #f0f4f8;
      transition: background-color 0.3s, color 0.3s;
    }
    #splash {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: #111;
      color: #fff;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
      z-index: 9999;
      animation: fadeOut 3s forwards;
    }
    @keyframes fadeOut {
      0% { opacity: 1; }
      90% { opacity: 0; }
      100% { opacity: 0; display: none; }
    }
    #editorContainer {
      width: 100%;
      height: 400px;
      border: 1px solid #ccc;
      border-radius: 8px;
      overflow: hidden;
    }
  </style>
</head>
<body class="text-gray-900">
  <div id="splash">🚀 ProDevStudio / LaunchPad</div>

  <div id="main" class="hidden">
    <header class="text-center py-6">
      <h1 class="text-4xl font-bold">LaunchPad</h1>
      <p class="text-lg">Open-source Code Refiner, Text Editor & Publisher</p>
      <p class="text-sm text-gray-500">Powered by ProDevStudio</p>
    </header>

    <div class="flex flex-col items-center justify-center px-4">
      <div class="flex flex-wrap justify-center space-x-2 mb-4">
        <button onclick="setMode('code')" class="bg-green-500 text-white px-4 py-2 rounded">Code Editor</button>
        <button onclick="setMode('text')" class="bg-blue-500 text-white px-4 py-2 rounded">Text Editor</button>
        <button onclick="saveDoc()" class="bg-yellow-500 text-white px-4 py-2 rounded">Save</button>
        <button onclick="toggleTheme()" class="bg-gray-800 text-white px-4 py-2 rounded">Toggle Theme</button>
        <button onclick="exportDoc('txt')" class="bg-purple-500 text-white px-4 py-2 rounded">Export .txt</button>
        <button onclick="exportDoc('html')" class="bg-red-500 text-white px-4 py-2 rounded">Export .html</button>
        <button onclick="exportDoc('md')" class="bg-indigo-500 text-white px-4 py-2 rounded">Export .md</button>
      </div>

      <div id="editorContainer"></div>

      <div class="mt-6 text-center">
        <h2 class="text-xl font-semibold">Ad Space</h2>
        <div class="border p-4 mt-2 w-full max-w-md">
          <p class="text-sm text-gray-600">Ad powered by ProDevStudio</p>
          <img src="https://via.placeholder.com/300x100" alt="ProDevStudio Ad" class="mx-auto mt-2">
        </div>

        <div class="mt-6">
          <h3 class="text-lg font-semibold">Support LaunchPad</h3>
          <p class="text-sm">Like what we do? Donate to keep LaunchPad growing!</p>
          <a href="#" class="mt-2 inline-block bg-pink-500 text-white px-4 py-2 rounded">Donate</a>
        </div>
      </div>
    </div>
  </div>

  <script>
    let editor;
    let mode = 'code';

    require.config({ paths: { vs: "https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.34.1/min/vs" } });
    require(["vs/editor/editor.main"], function () {
      editor = monaco.editor.create(document.getElementById("editorContainer"), {
        value: localStorage.getItem('launchpad_content') || "",
        language: "javascript",
        theme: "vs-dark",
        automaticLayout: true
      });
    });

    function setMode(newMode) {
      mode = newMode;
      const language = newMode === 'code' ? 'javascript' : 'plaintext';
      monaco.editor.setModelLanguage(editor.getModel(), language);
    }

    function saveDoc() {
      const content = editor.getValue();
      localStorage.setItem('launchpad_content', content);
      alert('Document saved locally.');
    }

    function exportDoc(format) {
      const content = editor.getValue();
      let blob;
      let filename = `launchpad_export.${format}`;
      if (format === 'html') {
        const html = `<!DOCTYPE html><html><head><meta charset='UTF-8'></head><body><pre>${content}</pre></body></html>`;
        blob = new Blob([html], { type: 'text/html;charset=utf-8' });
      } else if (format === 'md') {
        blob = new Blob([content], { type: 'text/markdown;charset=utf-8' });
      } else {
        blob = new Blob([content], { type: 'text/plain;charset=utf-8' });
      }
      saveAs(blob, filename);
    }

    function toggleTheme() {
      const currentTheme = editor._themeService._theme.themeName;
      const newTheme = currentTheme === 'vs-dark' ? 'vs-light' : 'vs-dark';
      monaco.editor.setTheme(newTheme);
    }

    window.onload = () => {
      const splash = document.getElementById('splash');
      const main = document.getElementById('main');
      setTimeout(() => {
        splash.style.opacity = 0;
        setTimeout(() => {
          splash.style.display = 'none';
          main.classList.remove('hidden');
        }, 500);
      }, 3000);
    }
  </script>
</body>
</html>
