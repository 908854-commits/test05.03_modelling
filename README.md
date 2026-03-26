# Van Gogh Correspondence Networks

This report proposes a data model and analytical framework for constructing a network representation of Vincent van Gogh’s social environment using his correspondence. The digital edition of Van Gogh’s letters provides structured metadata including sender, recipient, date, topic and type of letter. These elements allow the creation of a relational dataset that represents communication interactions between individuals. Using this information, a graph network can be constructed where persons are nodes and letters are edges connecting them. Network analysis techniques enable visualization of communication intensity, identification of central figures in Van Gogh’s correspondence, and examination of temporal and geographic patterns in his social interactions. The resulting model aims to represent the social, cultural, and artistic environment surrounding the artist.

## Dataset structure

This datasets presents ten letters from [vangoghletters.org](https://vangoghletters.org/vg/letters/let871/letter.html)

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

## Topic Modelling and Network Analysis

To allow a topic-based network analysis the raw topics idicated on the archive, for each letter, have been divided into three macro-categories, Relationships, War and Arts, as in the following example:

|letter ID       |Topic Raw                                               |Topic Category               |
|----------------|--------------------------------------------------------|-----------------------------|
|1               |The death of Mr van Gogh                                |Relationships                |
|2               |Decision to go to Auvers; Fourth attack in Saint-Rémy   |War                          |
|3               |Request to Russell to buy a painting from Gauguin       |Arts                         |

