# Facebook-Friend-Recommendation

# Business Problem: <br/>
  Given a directed social graph, we have to predict missing links to recommend friends/connnections/followers (Link Prediction in graph)<br/>
  
 # Data:<br/>
 
1. train.csv contains the directed social graph, represented in a 2-column csv (source_node, destination_node)<br/>
2. test.csv contains a list of nodes to recommend other nodes to in a 1-column csv (source_node) <br/>
Total number of Nodes/Vertices - 186220  <br/>
Total number of Edges/links - 9437519<br/>

# Machine Learning Problem: <br/>

 It is a Binary Classification Problem.  <br/>
 0 - No relation between them(No edge/Link)<br/>
 1 - Relationship exists(Existence of edge/Link)<br/>

# Business Objectives and Constraints: <br/>

    1. No low latency rate required.<br/>
    2. Predciting the probability of a link  is useful so as to recommend the highest probability links to a user.<br/>

# Performance Metrics: <br/>

  F1-Score  <br/>
  Confusion Matrix <br/>
  
  # Featurizations:<br/>  
  Jardac Distance,Cosine Distance,Page Rank,Shortest Path,Connected Components,Adar Index,HITS Score,Kartz centrality,SVD,weight features.<br/>
  
  # Models:<br/>
  
- Trained using randomised radom forest.<br/>
- Output : Train f1 score 0.9652533106548414,Test f1 score 0.9241678239279553<br/>
- Plot confusion matrix<br/>
- plotted roc-auc curve<br/>
