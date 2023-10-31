
<!DOCTYPE html>
<html>
<head>
    <title>Cannabis Sativa Clustering</title>
</head>
<body>
    <!-- Layout Description Section -->
    <div>
        <h1>Clustering of the Cannabis Sativa Literature with t-SNE and K-Means</h1>
        <p>
            This figure depicts the clustering patterns that emerged upon applying an unsupervised machine learning (ML) technique called natural language processing (NLP) to a comprehensive dataset of 5480 scientific publications on Cannabis sativa spanning from 1843 to 2024. Notably, documents with similarly themed abstracts tend to group together and are represented by nearby cluster points on the plot. By hovering over these cluster points, additional details such as 'Title', 'Authors', 'Journal', 'DOI', and 'Year' will be displayed. Furthermore, users may obtain detailed information about individual clusters by clicking twice on any right-side cluster point. The upper-right portion of the plot offers alternative ways to interact with the data.
        </p>
    </div>
    
    <!-- Plot Section -->
    <div>
        <h2>Clustering Plot</h2>
        <div id="scatter-plot"></div>
    </div>
    
    <script>
        // JavaScript code to load and display the plot
        fetch('scatter_plot.html')
            .then(response => response.text())
            .then(html => {
                document.querySelector('#scatter-plot').innerHTML = html;
            });
    </script>
</body>
</html>
