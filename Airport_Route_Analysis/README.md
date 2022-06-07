# Airport Route Network Analysis and New Flight Route Recommendation
## Introduction
If you are the airline businessman, you have to know how complexity of airport route network, and the influence of airport location in order to plan or launch the new commercial route to boost competitiveness in airline industry. The main solution is to apply social network analysis to visualize the holistic viewpoint in "Aerial or Satellite View" and measure the centrality indicator to formulate the airline hub strategy alonside with further available data such as number of passenger, geopolitics and sizing of airplane etc. Therefore, i would like to make a tools to measure preliminary recommendation with the "Open Triangle" algorithm to airline business owner. 
### DATASET
- Airport Database from Openflight [here](https://www.kaggle.com/datasets/divyanshrai/openflights-airports-database-2017)
- Route Network Database from Openflight [here](https://www.kaggle.com/datasets/divyanshrai/openflights-route-database-2014)
## Algorithm
- **Triadic closure** is a concept in social network theory and it is the property among three nodes A, B, and C (representing people, for instance), such that if a *strong tie* exists between A-B and A-C, there is a weak or strong tie between B-C. This property is too extreme to hold true across very large, complex networks, but it is a useful simplification of reality that can be used to understand and predict networks.

![image](https://user-images.githubusercontent.com/104628789/170211824-cb81ebb9-32dc-4005-99c9-a0171dd11b41.png)

- **In degree** :  the number of connections that point inward at a vertex. This indicator is used to measure *"the most incomiing flight airport"*.
- **Out Degree** : the number of connections that originate at a vertex and point outward to other vertices. This indicator is used to measure *"the most outgoing flight airport"*.
- **Degree Centrality** : the number of links incident upon a node. This indicator is used to measure *"the most connected airport"*.
- **Betweeness Centrality** : a way of detecting the amount of influence a node has over the flow of information in a graph. This indicator is used to measure *"the most transited airport"*.
- **Closeness Centrality** : a measure of the average shortest distance from each vertex to each other vertex. This indicator is used to measure *"the airport centrality with shortest path to another airport"*.
- **PageRank Centrality** : a way of ranking content, using links between them as a measure of importance.

## I. SOUTH EAST ASIA

![image](https://user-images.githubusercontent.com/104628789/170212631-7ad64604-a603-4640-8be3-36f1cb80c6c8.png)


![image](https://user-images.githubusercontent.com/104628789/170212548-7c061667-a707-47e7-bbaa-8b7b22cd75ba.png)

![image](https://user-images.githubusercontent.com/104628789/170212695-9645b295-65f9-440d-8845-86c40b0e5b91.png)

![image](https://user-images.githubusercontent.com/104628789/170212819-5b4ba37e-559f-4729-afd3-fcdd57f497e4.png)

![image](https://user-images.githubusercontent.com/104628789/170212875-df2a0d76-8a7e-4a1f-be01-f5501228838d.png)

### What are the top  5 airports with most incoming flights in South East Asia? 
- Singapore Changi
- Suvarnabhumi
- kuala lumpur
- Ninoy aquino
- Soekarno hatta 
### What are the top 5 airports with most outgoing flights in South East Asia? 
- Singapore Changi
- Suvarnabhumi
- kuala lumpur
- Ninoy aquino
- Soekarno hatta 
### What are the top 5 most connected airport in South East Asia? 
- Singapore Changi
- Suvarnabhumi
- kuala lumpur
- Ninoy aquino
- Soekarno hatta 
### What are the top 5 most transited airport in South East Asia? 
- Singapore Changi
- Suvarnabhumi
- Ninoy aquino
- kuala lumpur
- Soekarno hatta 
### What are the top 5 most centrality of South East Asia with shortest path to another airport?
- Suvarnabhumi
- Singapore Changi
- kuala lumpur
- Ninoy aquino
- Soekarno hatta 

#### Recommendation

- Kuala Lumpur   Malaysia to Hang Nadim   Indonesia
- Singapore Changi  Singapore to Hang Nadim   Indonesia
- Ninoy Aquino   Philippines to Don Mueang   Thailand
- Brunei   Brunei to Ngurah Rai (Bali)   Indonesia
- Phuket   Thailand to Tan Son Nhat   Vietnam

## II. ASIA PACIFIC

![image](https://user-images.githubusercontent.com/104628789/170213638-644e79dc-d3a5-488a-853d-51bf09871f6f.png)

![image](https://user-images.githubusercontent.com/104628789/170213695-14cf8d60-6873-4b16-8cfa-53c7690c108e.png)

![image](https://user-images.githubusercontent.com/104628789/170223554-ab5c1060-8ee7-48df-bb27-954ed7b17f8e.png)

![image](https://user-images.githubusercontent.com/104628789/170223485-f6132eb4-570b-482e-a104-fdfa499c758a.png)

![image](https://user-images.githubusercontent.com/104628789/170223762-54e89364-bc35-4d51-844b-6b2698761dd7.png)

### What are the top  5 airports with most incoming flights in Asia Pacific? 
- Beijing Capitol
- Shanghai Pudong
- Guangzhou Baiyun
- Incheon
- Singapore Changi
### What are the top 5 airports with most outgoing flights in Asia Pacific? 
- Beijing Capitol
- Shanghai Pudong
- Guangzhou Baiyun
- Incheon
- Singapore Changi
### What are the top 5 most connected airport in Asia Pacific? 
- Beijing Capitol
- Shanghai Pudong
- Guangzhou Baiyun
- Incheon
- Singapore Changi
### What are the top 5 most transited airport in Asia Pacific? 
- Singapore Changi
- Narita
- Sydney Kingsford Smith
- Singapore Changi
- Brisbane 
### What are the top 5 most centrality of Asia Pacific with shortest path to another airport?
- Beijing Capitol
- Narita
- Incheon
- Shanghai Pudong
- Suvarnabhumi

#### Recommendation

- Haikou Meilan   China to Incheon   South Korea
- Taiwan Taoyuan   Taiwan to Don Mueang   Thailand
- Liuting  China to Jeju   South Korea
- Beijing Capital   China to Don Mueang   Thailand
- Taiwan Taoyuan   Taiwan to Shanghai Hongqiao   China

## III.MIDDLE EAST AND SOUTH ASIA 

![image](https://user-images.githubusercontent.com/104628789/170214713-410809ff-70d1-4d55-b8ef-458e3cf83591.png)

![image](https://user-images.githubusercontent.com/104628789/170214817-96b29976-b086-4f08-9c8e-c904ae426a04.png)

![image](https://user-images.githubusercontent.com/104628789/170223853-7c155ac0-8db0-4d80-ac5a-4ead06c35ee9.png)

![image](https://user-images.githubusercontent.com/104628789/170223949-b577babb-6b4a-43c6-9c59-a0bf430a2503.png)

![image](https://user-images.githubusercontent.com/104628789/170224111-52b3de5e-319f-494f-9f40-6d03f5ffb478.png)

### What are the top  5 airports with most incoming flights in Middle East & South Asia? 
- Dubai
- Hamad
- India Gandhi
- Abu dhabi
- Chhatrapati Shivaji
### What are the top 5 airports with most outgoing flights in Middle East & South Asia? 
- Dubai
- Hamad
- India Gandhi
- Abu dhabi
- Chhatrapati Shivaji
### What are the top 5 most connected airport in Middle East & South Asia? 
- Dubai
- Hamad
- India Gandhi
- Abu dhabi
- Chhatrapati Shivaji
### What are the top 5 most transited airport in Middle East & South Asia? 
- Dubai
- Hamad
- India Gandhi
- Chhatrapati Shivaji
- Abu dhabi
### What are the top 5 most centrality of Middle East & South Asia with shortest path to another airport?
- Dubai
- Hamad
- Abu dhabi
- India Gandhi
- Chhatrapati Shivaji


#### Recommendation

- Netaji Subhash Chandra Bose   India Sharjah UAE
- Netaji Subhash Chandra Bose   India Abu Dhabi UAE
- Sardar Vallabhbhai Patel   India Bandaranaike Srilanka
- Sardar Vallabhbhai Patel   India Tribhuvan   Nepal
- Indira Gandhi   India New Islamabad   Pakistan

## IV. EUROPE

![image](https://user-images.githubusercontent.com/104628789/170225638-21470f9c-4ea8-46a0-a95a-c6d8ea0a685a.png)

![image](https://user-images.githubusercontent.com/104628789/170225689-d5b5ed7c-038c-4b45-8e49-3f4fd11458bd.png)

![image](https://user-images.githubusercontent.com/104628789/170225750-9d8bac0e-692e-4d6a-8220-8e0cadd773b3.png)

![image](https://user-images.githubusercontent.com/104628789/170225984-fbc1605c-38bf-4ec7-aa19-250a23cc2df2.png)

![image](https://user-images.githubusercontent.com/104628789/170226183-7a0b4fa3-8da6-441f-bf50-e32f55d87351.png)

### What are the top  5 airports with most incoming flights in Europe? 
- frankfurt am main
- charles de gaulle
- Amsterdam Schiphol
- Munich
- Domodedovo
### What are the top 5 airports with most outgoing flights in Europea? 
- frankfurt am main
- charles de gaulle
- Amsterdam Schiphol
- Munich
- Domodedovo

### What are the top 5 most connected airport in Europe? 
- frankfurt am main
- charles de gaulle
- Amsterdam Schiphol
- Munich
- Domodedovo
### What are the top 5 most transited airport in Europe? 
- charles de gaulle
- frankfurt am main
- Amsterdam Schiphol
- London Heathrow
- Domodedovo
### What are the top 5 most centrality of Europe with shortest path to another airport?
- frankfurt am main
- charles de gaulle
- London Heathrow
- Amsterdam Schiphol
- Munich

#### Recommendation

- Brussels South Charleroi  Belgium to London Stansted United Kingdom
- Berlin-Tegel  Germany to London Gatwick  United Kingdom
- Düsseldorf  Germany to Brussels  Belgium
- Málaga  Spain Nice-Côte d'Azur  France
- Berlin-Tegel  Germany Manchester  United Kingdom

## V. North America

![image](https://user-images.githubusercontent.com/104628789/170226774-4862e2cf-8a4a-490e-996a-0c5f9c7b07e1.png)

![image](https://user-images.githubusercontent.com/104628789/170226827-4d46ba43-6ddb-45e4-a352-253f140f822a.png)

![image](https://user-images.githubusercontent.com/104628789/170226900-55d9acbe-e6db-43af-a992-a474b2f89cf8.png)

![image](https://user-images.githubusercontent.com/104628789/170226960-47d10a7a-05d3-48c7-adc0-8b266726cbe0.png)

![image](https://user-images.githubusercontent.com/104628789/170227023-3e415b0d-588d-4bb0-82ac-2856fc5c6a83.png)

### What are the top  5 airports with most incoming flights in North America? 
- Hartsfield-Jackson
- Chicago O'Hare
- Dallas Fort Worth
- Bush houston
- Denver
### What are the top 5 airports with most outgoing flights in North America? 
- Hartsfield-Jackson
- Chicago O'Hare
- Dallas Fort Worth
- Bush houston
- Denver

### What are the top 5 most connected airport in North America? 
- Hartsfield-Jackson
- Chicago O'Hare
- Dallas Fort Worth
- Denver
- Bush houston

### What are the top 5 most transited airport in North America? 
- Ted Stevens Anchorage
- Los Angeles
- Chichago O'hare
- Seattle tacoma
- Lester B. Pearson
### What are the top 5 most centrality of North America with shortest path to another airport?
- Los angeles
- John F. Kennedy
- Lester B. Pearson
- Chichago O'hare
- Newark liberty

#### Recommendation

- Cancún   Mexico to McCarran   United States
- Lester B. Pearson   Canada to Chicago Midway   United States
- Cancún   Mexico to Tampa   United States
- Phoenix Sky Harbor   United States to Montreal / Pierre Elliott Trudeau Canada
- Cancún   Mexico San Diego   United States

## VI. South America

![image](https://user-images.githubusercontent.com/104628789/170227523-aba99246-8e03-4d5f-a91a-acd15d557f72.png)

![image](https://user-images.githubusercontent.com/104628789/170227570-29ef9a96-b95e-4844-ad84-8239a1a03915.png)

![image](https://user-images.githubusercontent.com/104628789/170227645-0c2fbdf2-3904-49e4-8c48-6fde28fdfe3b.png)

![image](https://user-images.githubusercontent.com/104628789/170227688-4db9d563-05bb-4864-beed-c90c050aaa67.png)

![image](https://user-images.githubusercontent.com/104628789/170227925-401b798b-08e8-41e9-94b1-9b417b7d6115.png)

### What are the top  5 airports with most incoming flights in South America? 
- André franco montoro
- el dorado
- jorge chavez
- Viracopos
- Tom jobim

### What are the top 5 airports with most outgoing flights in South America? 
- André franco montoro
- el dorado
- jorge chavez
- Viracopos
- Tom jobim

### What are the top 5 most connected airport in South America? 
- André franco montoro
- el dorado
- jorge chavez
- Viracopos
- Tom jobim


### What are the top 5 most transited airport in South America? 
- André franco montoro
- el dorado
- Arturo Merino Benítez
- jorge newbery
- jorge chavez

### What are the top 5 most centrality of South America with shortest path to another airport?
- André franco montoro
- Tom jobim
- jorge chavez
- Arturo Merino Benítez
- el dorado


#### Recommendation

- Jorge Newbery Airpark Argentina to Jorge Chávez  Peru
- Carrasco  /General C L Berisso  Uruguay to Hercíl Brazil
- Viracopos   Brazil to Ministro Pistarini   Argentina
- Jorge Newbery Airpark Argentina to Congonhas  Brazil
- Tancredo Neves   Brazil to Ministro Pistarini   Argentina

## VII. World

![image](https://user-images.githubusercontent.com/104628789/170228717-c0a831a5-663e-4802-9b87-069397555184.png)

![image](https://user-images.githubusercontent.com/104628789/170228771-781e4174-c6c4-4c64-bc69-092428c4c6f3.png)

![image](https://user-images.githubusercontent.com/104628789/170228884-89d3d737-68d6-42a6-b735-fbbf48a924f1.png)

![image](https://user-images.githubusercontent.com/104628789/170228941-83ead501-2c92-4c22-a99d-080da53a6856.png)

![image](https://user-images.githubusercontent.com/104628789/170229003-9c3286c9-38e2-40d1-86c0-41b3d435c5b9.png)

### What are the top  5 airports with most incoming flights in World? 
- Frankfurt
- charles de gaulle
- amsterdam schiphol
- istanbul
- Hartsfield-jackson
### What are the top 5 airports with most outgoing flights in World? 
- Frankfurt
- charles de gaulle
- amsterdam schiphol
- istanbul
- Hartsfield-jackson

### What are the top 5 most connected airport in World? 
- Frankfurt
- charles de gaulle
- amsterdam schiphol
- istanbul
- Hartsfield-jackson


### What are the top 5 most transited airport in World? 
- Ted Stevens Anchorage
- Los Angeles
- charles de gaulle
- Dubai
- Frankfurt

### What are the top 5 most centrality of World with shortest path to another airport?
- Frankfurt
- charles de gaulle
- London Heathrow
- Dubai
- Amsterdam schiphol

#### Recommendation
- Brussels South Charleroi  Belgium to London Stansted United Kingdom
- Düsseldorf  Germany to Brussels  Belgium
- Berlin-Tegel  Germany to London Gatwick  United Kingdom
- Málaga  Spain Nice-Côte d'Azur  France
- Frankfurt am Main  Germany London Gatwick  United Kingdom


## Notebook

you can find notebook [here](https://github.com/WarintornNawong/Portfolio/blob/main/Airport_Route_Analysis/Airport%20Route%20Network%20Analysis.ipynb)

