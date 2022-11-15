# Applications of graphical models to Web Analytics Data.

The objective of this project was to identify clusters of web users based on their behaviour while browsing a company's main website.

To do so, I created two types of graphs:
1. A collapsed graph where the nodes consisted only in the website's pages and the links were formed based on the occurrence that a user visited both the two pages considered. (Collapsed, Weighted based on the number of visits to the pages, Undirected)
2. A bipartite graph where the nodes consisted in both the website pages and the users' ID a the links were formed based on the occurrence that a user visited a specific page. (Bipartite, Undirected)

<img src="https://user-images.githubusercontent.com/49654710/201897648-33ad0a1b-2904-4a25-9713-5df94772e38e.png">

Given the created graphs, I was then able to apply two distinct clustering algorithms (Comunity Louvain and Core) to distinguish groups of similar nodes. This procedure was interesting to discover paths of action of the users that browse the website and to identify groups of users sharing similar behaviours.

Lastly, I applied Node2Vec to extract the embeddings associated to each node within the graph and I used these arrays as input to compute the cosine similarity between nodes. This process allowed me to create a similarity tool to understand the most similar pages based on the users' interactions with them and without considering any information about their content.

Thank you for you attention

Hope you enjoyed :)




