<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fling GUI</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        function toggleStatus() {
            const statusElement = document.getElementById('status');
            if (statusElement.innerText === 'Off') {
                statusElement.innerText = 'On';
                activateFlingScript();
            } else {
                statusElement.innerText = 'Off';
                deactivateFlingScript();
            }
        }

        function activateFlingScript() {
            console.log("Fling script activated");
            // Add your fling script activation code here
            // Example: document.getElementById('fling-element').classList.add('fling-active');
        }

        function deactivateFlingScript() {
            console.log("Fling script deactivated");
            // Add your fling script deactivation code here
            // Example: document.getElementById('fling-element').classList.remove('fling-active');
        }
    </script>
</head>
<body class="bg-gray-800 flex items-center justify-center min-h-screen">
    <div class="bg-gray-700 p-6 rounded-lg shadow-lg text-center w-64">
        <h1 class="text-white text-lg mb-4">Fling GUI</h1>
        <div class="bg-gray-600 p-2 rounded mb-4 cursor-pointer" onclick="toggleStatus()">
            <p id="status" class="text-gray-300">Off</p>
        </div>
        <p class="text-white">Credits: Vĩ script</p>
    </div>
</body>
</html>
