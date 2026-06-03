# New-project
First repo
<br>
Author - Mohd Samad
<!DOCTYPE html>
<html>
<head>
    <title>LocalStorage Demo</title>
</head>
<body>
    <h1>LocalStorage Data Storage</h1>
    
    <input type="text" id="dataInput" placeholder="Enter data">
    <button onclick="saveData()">Save</button>
    <button onclick="loadData()">Load</button>
    <button onclick="clearData()">Clear</button>
    
    <p id="output"></p>

    <script>
        // Save data
        function saveData() {
            const data = document.getElementById('dataInput').value;
            localStorage.setItem('myData', data);
            alert('Data saved!');
        }

        // Load data
        function loadData() {
            const data = localStorage.getItem('myData');
            document.getElementById('output').textContent = 'Stored: ' + data;
        }

        // Clear data
        function clearData() {
            localStorage.removeItem('myData');
            alert('Data cleared!');
        }
    </script>
</body>
</html>