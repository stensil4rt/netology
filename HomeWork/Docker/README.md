1. Установка Debian в VB
![image](https://user-images.githubusercontent.com/62753044/236879570-90e8fe06-b82a-4091-89df-27abef3f886c.png)

2. Добавление USER в root

![image](https://user-images.githubusercontent.com/62753044/236883894-6bcc3f11-c538-4795-9a2a-fa2d8afda5bd.png)

3.

![image](https://user-images.githubusercontent.com/62753044/236883917-5da00bf7-1d00-499e-a936-dc6bcabf8971.png)

4.
sudo apt update

![image](https://user-images.githubusercontent.com/62753044/236884778-14bda435-0733-47a5-81ac-4a397f7acaaa.png)

5.
sudo apt -y install ca-certificates curl gnupg lsb-release
![image](https://user-images.githubusercontent.com/62753044/236884916-459f49fc-9e95-47fe-bee7-a53fc3927dd7.png)

6.
curl -fsSL https://download.docker.com/linux/debian/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
![image](https://user-images.githubusercontent.com/62753044/236885009-e5b0b507-c415-43f5-9ce4-cda22ffda2a9.png)

7.
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/debian $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
![image](https://user-images.githubusercontent.com/62753044/236885084-0c4ff272-9ac6-4d86-a5d9-5c86bbd954e4.png)
8.
![image](https://user-images.githubusercontent.com/62753044/236885222-e716cc90-7e8f-4cd9-b7ba-93da5a849739.png)
9.
![image](https://user-images.githubusercontent.com/62753044/236885448-68ad8fef-12f9-4d83-a068-51741f6c5efd.png)
10.
sudo systemctl start docker
sudo systemctl status docker
Проверка:
![image](https://user-images.githubusercontent.com/62753044/236885570-b4e805d0-a3e3-4813-afb7-93aa38cf95ce.png)

11.
sudo groupadd docker
sudo usermod -aG docker $USER
![image](https://user-images.githubusercontent.com/62753044/236886506-7439a6bc-8e59-4e30-92da-92bdb2073a6e.png)
12.
После добавления пользователя необходимо перелогиниться в системе.
![image](https://user-images.githubusercontent.com/62753044/236886651-159c7f5a-fff5-4ea7-bc2b-cfc0a9e80914.png)
13.
Запуск образа hello-world.
docker run hello-world
![image](https://user-images.githubusercontent.com/62753044/236886881-bf846a1c-d5b5-4f50-a071-17f54f6f4198.png)

14.


