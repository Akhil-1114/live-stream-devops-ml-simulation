01.) remove unwanted repositories

gh auth refresh -h github.com -s delete_repo

gh repo delete https://github.com/Akhil-1114/live-stream-devops-ml-simulation --confirm --yes

02.) check repositories already present

$ gh repo list Akhil-1114

03.) create repository

$ gh repo create live-stream-devops-ml-simulation --public --confirm

04.) create folder locally git

$ mkdir live-stream-devops-ml-simulation

05.) get into folder locally git

$ cd live-stream-devops-ml-simulation

06.) set branch

$ git init -b main

07.) connect local repository to remote github

$ git remote add origin https://github.com/Akhil-1114/live-stream-devops-ml-simulation.git

# Setup GitHub directory
cd live-stream-devops-ml-simulation

touch README.md 
touch .gitignore
mkdir day01
cd day01
mkdir terraform
mkdir jenkins


create jenkins
check docker
docker --version


check docker info
docker info

run test container
docker run hello-world

check all containers
docker ps

check running containers
docker ps -a


get running container ids
docker ps -q

remove stopped containers
docker rm e59dced2e649

install jenkins image
docker run -d -p 8080:8080 -p 50000:50000 --name jenkins jenkins/jenkins:lts


| Step                         | What Happens                                                                       | Time Estimate                                     |
| ---------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------- |
| 🔽 **Image Pull**            | Docker downloads `jenkins/jenkins:lts` image (≈ 500–700 MB) if it's **not cached** | **2–10 minutes** (depends on your internet speed) |
| ⚙️ **Container Start**       | Jenkins initializes for the first time (installs plugins, sets up home dir)        | **30 sec – 2 min**                                |
| ✅ **Total First-Time Setup** | Image pull + container init                                                        | **\~3–12 minutes**                                |


monitor real time installation
docker logs -f jenkins

terraform -v

docker build -t ml-base:latest .

docker build -t ml-base:latest . | tee ../../logs/docker-build-ml-base.log

echo "Updated at $(date)" >> logs/day01-commands.md


git status

git remote -v

git log

git log --oneline

git add .

git commit -m "."

git push -u origin main
