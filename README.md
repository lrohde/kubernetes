# kubernetes
Instruções para um cluster Kubernetes

#Rolling Update
Para atualizar uma imagem primeiramente cetifique-se de que há a instrução imagePullPolicy: Always dentro do deloyment, após isso, basta executar kubectl set image deployment/my-deployment mycontainer=myimage:latest.

Também é possível controlar o tempo em que os pods levarão para ser encerados através da instrução terminationGracePeriodSeconds, também dentro do deployment.
