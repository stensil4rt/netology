<p align="center"> **Задание 1.** </p>
1.	
ParrotOS
![alt](https://user-images.githubusercontent.com/62753044/224276548-684fa5de-ef0d-4b20-8b34-9daf0f330d47.png)
4.
![image](https://user-images.githubusercontent.com/62753044/224276629-3e7750b5-79ea-440a-8ebd-8388b62653d6.png)
5.
![image](https://user-images.githubusercontent.com/62753044/224276661-48bbd31a-c740-40d4-aaf4-b4d3e5e62c09.png)
PKGS-7392 - Vulnerable packages
![image](https://user-images.githubusercontent.com/62753044/224276696-1b3899a5-6f9b-434a-b1bb-9ca0c64db757.png)
NETW-2705 - Properly functioning name servers
![image](https://user-images.githubusercontent.com/62753044/224276726-929819fc-216f-49b7-b232-5c54ea01b22a.png)
FIRE-4512 - Empty iptables ruleset
![image](https://user-images.githubusercontent.com/62753044/224276760-7e5ff804-56ba-44f4-83f3-ab47bc4ef7d9.png)
6. Выводы: В целом ОС защищена. При первом запуске необходимо было провести подновление всей системы (пакетов), также настроить DNS и iptables.

<p align="center"> **Задание 2.** </p>
1.
![image](https://user-images.githubusercontent.com/62753044/224276849-9d17272d-115d-460b-8931-2ba43578f095.png)
2.
![image](https://user-images.githubusercontent.com/62753044/224276875-3df18322-59a9-4a90-8bfb-4bafba24cc09.png)
3.
![image](https://user-images.githubusercontent.com/62753044/224276921-86fdc3c7-5961-428b-b3a3-2363c4c0d57a.png)
4.
![image](https://user-images.githubusercontent.com/62753044/224276954-1f58e956-1cb9-491b-bdfe-0de74fab7072.png)
5.
- Asus RT-AC1200
- Service Info: OS: Linux; Device: WAP; CPE: cpe:/o:linux:linux_kernel, cpe:/h:asus:rt-ac1200
- 4 
22/tcp    open  ssh     Dropbear sshd 2020.81 (protocol 2.0)
53/tcp    open  domain  dnsmasq 2.85-50ccf9c5852729a68a0359025cd3bda080acfc39
80/tcp    open  http    Asus RT-AC1200 WAP http config
28723/tcp open  upnp    MiniUPnP 2.1.20191006 (UPnP 1.1)
- ssh, http («WEB-морда») – можно было бы перевести на сертификат (https:443), но внктри сети этого не надо, DNS, функция UPnP
6.
 Все версии актуальны, все включено что нужно.

<p align="center"> **Задание 3. ** </p>
1.
![image](https://user-images.githubusercontent.com/62753044/224277716-f7556fcf-3fbe-42e1-a857-915150791ae7.png)
2. -
3. -
4.
![image](https://user-images.githubusercontent.com/62753044/224277787-b5909538-d889-487c-87bf-3753c3533c90.png)
5.
![image](https://user-images.githubusercontent.com/62753044/224277815-c5a1a30d-932e-4307-ba0f-5ea2fdd54017.png)
6. -
7. Анализ:
DNS запросы,
![image](https://user-images.githubusercontent.com/62753044/224277907-5cc77ef3-f1b0-48e7-8726-051b4e5e2573.png)
Идет рукопожатие,
![image](https://user-images.githubusercontent.com/62753044/224277988-aabad661-7d5a-4f9e-837f-f568cdb1e41e.png)
и т.д.
8. Выводы: Информация ходит та что и должна, «левых» подключений нет.
