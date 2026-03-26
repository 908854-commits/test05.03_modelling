# test05.03_modelling
This datasets presents ten letters from vangoghletters.org (https://vangoghletters.org/vg/letters/let871/letter.html)

The chosen categories are:
- ID
- Date
- Year
- Location
- From (Sender)
- To (Reciver)
- Topic
- Full Text (Boolean, False = Fragment)
- Telegram (Boolan, False = Letter)

'Na' value was used to indicate not available data

Title: Data Modeling Structure:Van Gogh Correspondence Networks 
 Professor: Emmanuela Carbé
 Students:Aim Batalova, Natalia Pierzchala
 Date: 10 March 2026

Van Gogh Social Network: Modeling Correspondence Networks from Digital Letters
Abstract
This report proposes a data model and analytical framework for constructing a network representation of Vincent van Gogh’s social environment using his correspondence. The digital edition of Van Gogh’s letters provides structured metadata including sender, recipient, date, and place for each letter. These elements allow the creation of a relational dataset that represents communication interactions between individuals. Using this information, a graph network can be constructed where persons are nodes and letters are edges connecting them. Network analysis techniques enable visualization of communication intensity, identification of central figures in Van Gogh’s correspondence, and examination of temporal and geographic patterns in his social interactions. The resulting model aims to represent the social, cultural, and artistic environment surrounding the artist.


The Main Idea of Analysis
The central goal of this project is to model the social network of Vincent van Gogh using his correspondence as relational data. The digital edition of Van Gogh’s letters contains extensive correspondence between Van Gogh and various individuals including family members and artists. The collection includes letters to his brother Theo van Gogh and to artists such as Paul Gauguin and Emile Bernard, among others. Each letter entry contains descriptive metadata such as sender, recipient, date, place of writing.

The analysis addresses several research questions:
Who were the key individuals in Van Gogh’s correspondence network?
What types of relationships dominate the communication network?
How did Van Gogh’s communication network evolve over time?
How does the geographic distribution of letters correspond to phases of Van Gogh’s artistic career?
