# edgeTOgml
Code Snippet to convert a graph data from edgelist format to gml format

# Convert a graph data from edgelist format to gml format
# run in  Colab

import networkx as nx


G= nx.read_edgelist('1684.edges')


n = G.number_of_nodes()

m = G.number_of_edges()

print("Number of nodes : %d" % n)

print("Number of edges : %d" % m)

nx.write_gml(G, "1684inGML.gml") # file in gml format is created in your pwd
