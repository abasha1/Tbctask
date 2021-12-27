# Tbctask
Tbctask
![image](https://user-images.githubusercontent.com/51801315/147501619-5c14088b-1c53-4fdb-8c60-32ad06b0229e.png)



დავალების შესასრულებლად: ლოკალურად Virtual Box-ში შევქმენი ვირტუალური მანქანა - Linux-სის ოპერაციულ სისტემაზე.თავდაპირველად დავაყენე კუბერნეტესი(K3s)
![image](https://user-images.githubusercontent.com/51801315/147501634-2509f935-a96e-480f-9ec7-d9d71f417a45.png)



შემდეგ შევქმენი Node-სახელად “NIKA” D 
![image](https://user-images.githubusercontent.com/51801315/147501652-2c2bb4c1-4bfe-4a10-a015-c2764a6a79f5.png)



ამის შემდეგ შევქმენი ფაილები შესაბამისი კონფიგურაციით ფაილი შესაბამისი კონფიგურაციით,  nginx_deployment.yaml,
 ასევე შევქმენი nginx_service.yaml ფაილი Network კონფიგურაციისთვის და ასევე  nginx_pvc.yaml შევქმენი (Provisioning-ის მიზნით) 
![image](https://user-images.githubusercontent.com/51801315/147501701-de60ab12-0195-4282-a504-38006f572483.png)



ასევე დავაინსტალირე HELM-ი და შევქმენი დეფლოიმენთისთვის საჭირო ფაილები შესაბამისი კონფიგურაციით.. დავაყენე რედისი.



![image](https://user-images.githubusercontent.com/51801315/147501714-ade1c448-5e99-4850-b228-99387ebd4a1f.png)


![image](https://user-images.githubusercontent.com/51801315/147501720-f92de426-c81e-44e4-99e6-0e6f91f75e32.png)


შემდეგ ასევე დავაინსტალირე Docker-ი, და გადავწყვიტე redis- ით და node.js-ით  აპლიკაციის გაშვება კონტეინერში .


![image](https://user-images.githubusercontent.com/51801315/147501733-32b80122-17c8-4375-99af-a8684c7ae7b4.png)


![image](https://user-images.githubusercontent.com/51801315/147501735-d5434bb1-2215-44a7-91f9-c8df29d5b423.png)


მსგავსი რაღაც გამომივიდა.( Count-ს უკეთებს გვერდის განახლებისას/რექუესთისგაგზავნისას)
![image](https://user-images.githubusercontent.com/51801315/147501746-0f1109b8-b147-45e3-96a3-b3ff0ee9b9bb.png)


Helm-ის დახმარებით დავაყენე Prometheus-ი და Grafana-ა, კლასტერის მონიტორინგისთვის.

![image](https://user-images.githubusercontent.com/51801315/147501774-35072320-6053-40cc-902b-f93b5af75bf9.png)

ამის შემდეგ გავაკეთე Port-Forward-ი


![image](https://user-images.githubusercontent.com/51801315/147501754-a429289d-e3f1-4f92-a658-e4fe37600d9e.png)


![image](https://user-images.githubusercontent.com/51801315/147501799-9c8aa95c-e4a1-4c3f-b3dd-695e551b83eb.png)

![image](https://user-images.githubusercontent.com/51801315/147501860-00e94375-ae8a-4d07-827f-42969729c479.png)

შემდეგ დავალების მიხედვით დავაინსტალირე ISTIO.

![image](https://user-images.githubusercontent.com/51801315/147501877-ed409069-f24d-460a-9a0e-62e322f353f9.png)

ISTIO-ს დაინსტალირების შემდეგ Deployment-გავუკეთე შემდეგ სერვისებს როგორიცააJAGER,Grafana,Prometheus,Kiali,Zipkin


![image](https://user-images.githubusercontent.com/51801315/147501922-f8223b31-a9ce-4a28-8733-5084d5e0af95.png)


![image](https://user-images.githubusercontent.com/51801315/147501924-988e3346-8e98-457e-a851-6fcdc2c86266.png)

შემდეგ იმისთვის რომ აღნიშნული სერვისი ყოფილიყო წვდომადი(კლასტერისგარედან), გავაკეთე Port-Forward-ი.

![image](https://user-images.githubusercontent.com/51801315/147501992-53a133ed-4619-4f86-a7a4-31d52b1b3fb6.png)


![image](https://user-images.githubusercontent.com/51801315/147502002-b47c87d8-f06b-46a3-af8f-fb589482afaf.png)


![image](https://user-images.githubusercontent.com/51801315/147502008-578161ef-383e-45f9-8662-b4dcea669876.png)

HELM-ის დახმარებით დავაყენე Haproxy Kubernetes-ingress  

![image](https://user-images.githubusercontent.com/51801315/147502030-c506054a-2cc3-410f-98b2-a8eba0701371.png)






