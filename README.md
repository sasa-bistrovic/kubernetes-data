<p><b><font face="Arial" size="4">Procedure for starting the project:</font></b></p>
<p><b><font face="Arial">1. You need to have docker desktop and minikube installed and kubernetes running.</font></b></p>

<p><b><font face="Arial">2. Clone the project from github.com with the command:</font></b></p>

<p><font face="Arial">$ git clone https://github.com/sasa-bistrovic/kubernetes-data.git</font></p>

<p><b><font face="Arial">3. In the "/kubernetes-data" folder, run the command:</font></b></p>

<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">minikube config set cpus 6</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">minikube config set memory 8000</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">minikube start</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">minikube kubectl -- apply -f kubernetes.yaml</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">minikube kubectl -- get pods</font></p>

<p><b><font face="Arial">4. After running the containers inside kubernetes run the command:</font></b></p>

<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">minikube service spring-boot-kafka --url</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">http&#58;//192.168.59.103&#58;32433</font></p>

<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">minikube service spring-boot-rabbitmq --url</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">http&#58;//192.168.59.103&#58;32222</font></p>

<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">minikube service spring-boot-elasticsearch --url</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">http&#58;//192.168.59.103&#58;31157</font></p>

<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">minikube service spring-boot-redis --url</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font face="Arial">http&#58;//192.168.59.103&#58;30364</font></p>

<p><b><font face="Arial">5. Here is picture from react-crud-kafka and spring-boot-kafka URL "http&#58;//192.168.59.103&#58;32433":</font></b></p>

<font face="Arial">

<img src="https://github.com/sasa-bistrovic/kubernetes-data/blob/main/kafka-spring-boot-react-crud.png"></img>

</font>

<p><b><font face="Arial">6. Here is picture from react-crud-rabbitmq and spring-boot-rabbitmq URL "http&#58;//192.168.59.103&#58;32222":</font></b></p>

<font face="Arial">

<img src="https://github.com/sasa-bistrovic/kubernetes-data/blob/main/rabbitmq-spring-boot-react-crud.png"></img>

</font>

<p><b><font face="Arial">7. Here is picture from react-crud-elasticsearch and spring-boot-elasticsearch URL "http&#58;//192.168.59.103&#58;31157":</font></b></p>

<font face="Arial">

<img src="https://github.com/sasa-bistrovic/kubernetes-data/blob/main/elasticsearch-spring-boot-react-crud.png"></img>

</font>

<p><b><font face="Arial">8. Here is picture from react-crud-redis and spring-boot-redis URL "http&#58;//192.168.59.103&#58;30364":</font></b></p>

<font face="Arial">

<img src="https://github.com/sasa-bistrovic/kubernetes-data/blob/main/redis-spring-boot-react-crud.png"></img>

</font>
