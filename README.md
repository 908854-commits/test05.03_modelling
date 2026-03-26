# Van Gogh Correspondence Networks

This report proposes a data model and analytical framework for constructing a network representation of Vincent van Gogh’s social environment using his correspondence. The digital edition of Van Gogh’s letters provides structured metadata including sender, recipient, date, topic and type of letter. These elements allow the creation of a relational dataset that represents communication interactions between individuals. Using this information, a graph network can be constructed where persons are nodes and letters are edges connecting them. Network analysis techniques enable visualization of communication intensity, identification of central figures in Van Gogh’s correspondence, and examination of temporal and geographic patterns in his social interactions. The resulting model aims to represent the social, cultural, and artistic environment surrounding the artist.

## Dataset structure

This datasets presents ten letters from [vangoghletters.org](https://vangoghletters.org/vg/letters.html)

The chosen categories are:
- ID
- Date
- Year
- Location
- From (Sender)
- To (Reciver)
- Topic Raw
- Topic Cadegory
- Full Text (Boolean, False = Fragment)
- Telegram (Boolan, False = Letter)

> **Note:** The **'Na'** value was used to indicate not available data

## Dataset Use

Once the network is constructed, several analytical methods can be applied.

**Community Detection** identifies clusters of communication. Possible subgroups: Family correspondence, Professional communication, Other forms of interaction. These clusters reveal social and professional groups in Van Gogh’s environment. 

**Degree Centrality** measures the number of connections associated with each node. This identifies the most central figures in the correspondence network. For example, frequent correspondents such as Van Gogh’s brother Theo form highly connected nodes.

**Temporal Analysis** letters are grouped by time periods. This allows analysis of communication intensity by year and shifts in Van Gogh’s social network over time. Temporal segmentation reveals phases of active correspondence.

**Geographic Analysis** by linking letters to places, the spatial distribution of correspondence can be analyzed. This reveals where Van Gogh was writing from and geographic spread of his communication network. Geographic analysis connects correspondence patterns with stages of Van Gogh’s artistic career.

**Topic Modelling** analyse the topics presented in the letters, considering three macro-catgories it's possible to sum up the different subjects contained in the texts. 

## Topic Modelling and Network Analysis

To allow a topic-based network analysis the raw topics idicated on the archive, for each letter, have been divided into three macro-categories, Relationships, War and Arts, as in the following example:

|letter ID       |Topic Raw                                               |Topic Category               |
|----------------|--------------------------------------------------------|-----------------------------|
|1               |The death of Mr van Gogh                                |Relationships                |
|2               |Decision to go to Auvers; Fourth attack in Saint-Rémy   |War                          |
|3               |Request to Russell to buy a painting from Gauguin       |Arts                         |
