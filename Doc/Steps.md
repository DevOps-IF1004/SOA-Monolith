# MenOps

### Steps 
1. Decompose SOA-Monolith (this repository) in **PEDIDO service** and **CLIENTE service**, and documenting the Architectural Design Decisions;
2. Write the verification of **Cliente** during recording of a new **Pedido**;
3. Write automated tests (Unit Tests);
4. Pass tests trough pipeline (https://circleci.com/ or Jenkins) using docker;
5. Deploy Services on Google Cloud or Amazon AWS;
6. Monitor the the record of new **pedidos** with Elastic Search;
7. Replicate PEDIDO service (>2 instances) and support availability of ecosystem;


### Teacher acceptance tests

* Step 1.a: The presentation of 2 repositories with the source code of microservices components; |Done|
* Step 1.b: The Technical Documentation of architectural decisions; |Done|
* Step 2: The presentation of the verification at runtime; | Done |
* Step 3: The presentation of source code of Unit Tests; | --- |
* Step 4 & 5: Execution of pipeline until deployment; | --- |
* Step 6: Show kibana monitoring the recording of new **pedidos**  | --- |
* Step 7: "simulate" a **PEDIDO service** (>2 instances) problem and the automated execution of the selfhealing;  | --- |



### Explanation
* Step 1.b: Foi separado em dois respositórios, utilizando portas diferentes. Onde o cliente passou a escutar na porta 8090, e o pedido na porta 8081. Como ambos já estava se comunicando através de uma API rest, então apenas separamos os códigos, os colocando em repositórios diferentes.

