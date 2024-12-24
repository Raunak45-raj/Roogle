<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Roogle</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f8f9fa;
            margin: 0;
            padding: 0;
        }
        .logo {
            font-size: 3rem;
            font-weight: bold;
            color: #4285F4;
            margin-top: 100px;
        }
        .logo span {
            color: #EA4335;
        }
        .search-box {
            margin-top: 50px;
        }
        .search-input {
            width: 50%;
            padding: 10px;
            font-size: 1.2rem;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        .search-button {
            padding: 10px 20px;
            font-size: 1.2rem;
            background-color: #4285F4;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        .search-button:hover {
            background-color: #357AE8;
        }
        .news-section {
            margin-top: 50px;
            text-align: left;
            padding: 20px;
            background-color: #fff;
            border-top: 1px solid #ddd;
        }
        .news-section h2 {
            font-size: 1.5rem;
            color: #333;
        }
        .news-item {
            margin: 10px 0;
            font-size: 1rem;
            color: #555;
        }
        .news-item a {
            text-decoration: none;
            color: #4285F4;
        }
        .news-item a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="logo">
        R<span>oo</span>gle
    </div>
    <div class="search-box">
        <input type="text" id="searchInput" class="search-input" placeholder="Search Roogle...">
        <button class="search-button" onclick="searchRoogle()">Search</button>
    </div>

    <div class="news-section">
        <h2>Latest News</h2>
        <div class="news-item">
            <a href="https://www.example.com/news1" target="_blank">Breaking: Technology advances in 2024</a>
        </div>
        <div class="news-item">
            <a href="https://www.example.com/news2" target="_blank">Economy Update: Markets soar to new heights</a>
        </div>
        <div class="news-item">
            <a href="https://www.example.com/news3" target="_blank">Sports: The most exciting game of the year!</a>
        </div>
        <div class="news-item">
            <a href="https://www.example.com/news4" target="_blank">Entertainment: Upcoming blockbuster movies</a>
        </div>
    </div>

    <footer>
        <p>Powered by Roogle | Just for Fun!</p>
    </footer>

    <script>
        function searchRoogle() {
            const query = document.getElementById('searchInput').value;
            if (query) {
                const url = `https://www.google.com/search?q=${encodeURIComponent(query)}`;
                window.open(url, '_blank');
            } else {
                alert("Please enter a search term!");
            }
        }
    </script>
</body>
</html>

