---


---

<p>Recommendation System based on Robust Continuous Clustering</p>
<h2 id="section"></h2>
<p>The main goal of this project is to design a movie recommendation system based on RCC (Robust Continuous Clustering), and to compare the results with the system based on k-means method.</p>
<h2 id="dataset">DataSet</h2>
<p><a href="https://grouplens.org/datasets/movielens/">MovieLens 10M dataset:</a><br>
contains four files: Users, Movie, Links, and Tags, in this project, all four files are used.</p>
<h2 id="recommendation-engine">Recommendation Engine</h2>
<h3 id="content-based-filtering">Content based filtering:</h3>
<p>Uses item vector (movies’ genres and tags and other basic information), and profile vector ( the past behaviors of the users, i.e. ratings of the movies).</p>
<h3 id="data-clustering">Data Clustering:</h3>
<ul>
<li>The recommendation system uses RCC to accomplish the data clustering task.  <a href="https://www.pnas.org/content/114/37/9814">https://www.pnas.org/content/114/37/9814</a></li>
<li>In this project I used the python implementation of RCC. <a href="https://github.com/yhenon/pyrcc">https://github.com/yhenon/pyrcc</a></li>
<li>Generally, to compute on a large data set requires a huge amount of resources, and compare to other clustering algorithms, this RCC could achieve a higher accuracy and scale efficiently to high dimensions and large data set.</li>
<li>To have a better sense of how this algorithm works, I also have designed a recommendation system based on k-means, and have compared  the results between these two algorithms.</li>
</ul>
<h3 id="main-steps">Main steps:</h3>
<ul>
<li>Formatted the data and understand them before any process</li>
<li>Have a list of the unique <strong>genres</strong>, then create dummy variables for later use.</li>
<li>And create feature vectors for all the <strong>tags</strong> as well, for later use.</li>
<li>K-means clustering.</li>
<li>Robust Continuous Clustering.</li>
<li>Recommend movies.</li>
</ul>

