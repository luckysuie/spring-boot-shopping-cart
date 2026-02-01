LakshmiNarayana@lucky:~/spring-boot-shopping-cart$ history
    1  docker --version
    2  docker ps
    3  docker build -t shopcart -f docker/Dockerfile .
    4  sudo docker pull sonarqube
    5  docker run -d -p 9000:9000 sonarqube
    6  sudo apt update
    7  mvn clean verify sonar:sonar   -Dsonar.projectKey=spring-boot-shopping-cart   -Dsonar.host.url=http://20.219.152.209:9000   -Dsonar.login=sqa_66ebd065f1f6f0941e3ef8c2a25ccd8f0733800e   -DskipTests
    8  hostory
    9  history
   10  ls
   11  sudo apt update
   12  curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
   13  az --version
   14  az login
   15  az login --use-device-code
   16  az account show
   17  az acr login --name luckyregistry
   18  docker tag shopcart luckyregistry.azurecr.io/shopcart:v1
   19  docker images | grep shopcart
   20  docker push luckyregistry.azurecr.io/shopcart:v1
   21  sudo apt update
   22  ls
   23  sudo apt install tree
   24  ls
   25  cd helm/
   26  tree
   27  cd t
   28  cd shopping-cart/
   29  cd templates/
   30  ks
   31  ls
   32  sudo apt update
   33  sudo snap install --classic kubectl
   34  kubectl version --client
   35  az aks get-credentials   --resource-group lucky   --name lucky-aks-cluster11   --overwrite-existing
   36  kubectl get nodes
   37  az aks update   --resource-group lucky   --name lucky-aks-cluster11   --attach-acr luckyregistry
   38  kubectl create namespace shopping-cart
   39  ls
   40  cd ..
   41  ls
   42  cat values.yaml
   43  grep -n "server.port" src/main/resources/application.properties
   44  cd
   45  cd s
   46  cd spring-boot-shopping-cart/
   47  grep -n "server.port" src/main/resources/application.properties
   48  history
   49  cd helm/
   50  ls
   51  cd shopping-cart/
   52  ls
   53  vi values.yaml
   54  cat Chart.yaml
   55  cd templates/
   56  ls
   57  cat _helpers.tpl hpa.yaml config.yaml deployment.yaml service.yaml ingress.yaml
   58  vi config.yaml
   59  vi deployment.yaml
   60  vi service.yaml
   61  vi hpa.yaml
   62  cd
   63  sudo pat update
   64  sudo apt update
   65  curl https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3 | bash
   66  helm version
   67  kubectl get nodes
   68  helm list -n shopping-cart
   69  cd spring-boot-shopping-cart/
   70  ls
   71  cd helm/
   72  ls
   73  cd shopping-cart/
   74  cat Chart.yaml
   75  kubectl get ns
   76  helm lint .
   77  helm template shopping-cart-blue . -n shopping-cart | head -n 40
   78  helm upgrade --install shopping-cart-blue .   -n shopping-cart   --set color=blue   --set service.activeColor=blue
   79  kubectl get pods
   80  kubectl get pods -n shopping-cart
   81  kubectl get svc -n shopping-cart
   82  kubectl describe pod -n shopping-cart-blue-5d95bcc456-glqsk
   83  kubectl describe pod -n shopping-cart shopping-cart-blue-5d95bcc456-glqsk
   84  cat values.yaml
   85  vi values.yaml
   86  helm upgrade shopping-cart-blue . -n shopping-cart
   87  kubectl get pods -n shopping-cart -w
   88  kubectl describe pod -n shopping-cart shopping-cart-blue-7db569cfc8-r6c4f | tail -n 80
   89  kubectl get all
   90  kube ctl get ns
   91  kubectl get ns
   92  kubectl get po -n shopping-cart
   93  kubectl get svc -n shopping-cart
   94  cd
   95  cd spring-boot-shopping-cart/
   96  ls
   97  mvn clean package -DskipTests
   98  docker build -t shopcart:v2 -f docker/Dockerfile .
   99  docker tag shopcart:v2 luckyregistry.azurecr.io/shopcart:v2
  100  ocker push luckyregistry.azurecr.io/shopcart:v2
  101  docker push luckyregistry.azurecr.io/shopcart:v2
  102  cd ~/spring-boot-shopping-cart/helm/shopping-cart
  103  helm upgrade --install shopping-cart-green . -n shopping-cart   --set color=green   --set service.activeColor=blue   --set image.tag=v2
  104  cd h
  105  ls
  106  cd templates/
  107  ls
  108  cd ..
  109  ls
  110  cd templates/
  111  ls
  112  cat config.yaml
  113  vi config.yaml
  114  ls
  115  cat deployment.yaml
  116  vi config.yaml
  117  ls
  118  vi deployment.yaml
  119  vi config.yaml
  120  cd
  121  cd ~/spring-boot-shopping-cart/helm/shopping-cart
  122  helm upgrade shopping-cart-blue . -n shopping-cart
  123  kubectl delete configmap -n shopping-cart shopping-cart-config
  124  helm upgrade --install shopping-cart-green . -n shopping-cart   --set color=green   --set service.activeColor=blue   --set image.tag=v2
  125  ls
  126  cd templates/
  127  ls
  128  vi service.yaml
  129  vi v
  130  ls
  131  cd ..
  132  vi values.yaml
  133  ls
  134  cd templates/
  135  ls
  136  vi service.yaml
  137  cd ~/spring-boot-shopping-cart/helm/shopping-cart
  138  helm upgrade shopping-cart-blue . -n shopping-cart
  139  helm upgrade --install shopping-cart-green . -n shopping-cart   --set color=green   --set service.create=false   --set image.tag=v2
  140  helm upgrade shopping-cart-blue . -n shopping-cart --set service.activeColor=green
  141  kubectl get endpoints -n shopping-cart shopping-cart-svc -o wide
  142  kubectl get pods -n shopping-cart -o wide
  143  kubectl get hpa -n shopping-cart
  144  cd
  145  ls
  146  cd spring-boot-shopping-cart/
  147  git add .
  148  git commit -m "Worked Code"
  149  git push
  150  history
  151  sudo apt update
  152  sudo apt-get install wget apt-transport-https gnupg lsb-release -y
  153  wget -qO - https://aquasecurity.github.io/trivy-repo/deb/public.key | sudo apt-key add -
  154  echo deb https://aquasecurity.github.io/trivy-repo/deb $(lsb_release -sc) main | sudo tee -a /etc/apt/sources.list.d/trivy.list
  155  sudo apt-get update
  156  sudo apt-get install trivy -y
  157  trivy --version
  158  vi azure-pipelines.yml
  159  git add .
  160  git commit -m "Added Pipeline"
  161  git push
  162  trivy image --severity HIGH,CRITICAL --exit-code 1 shopcart
  163  history
