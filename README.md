# Deployment Guide
1. **Use terraform configuration**
    ```sh
    terrafrom init
    terraform apply
    ```
## OpenVPN

1. **SSH log in to VM**
    ```sh
    ssh testadmin@<public_ip>
    ```

2. **Install updates and set the correct time**
    ```sh
    apt update
    apt upgrade
    apt install tzdata
    dpkg-reconfigure tzdata
    ```

3. **To install Access Server on your Linux server, run this command:**
    ```sh
    bash <(curl -fsS https://as-repository.openvpn.net/as/install.sh)
    ```

4. **Find your login and password to Admin UI. Exomple:**
    (C:\projects terraform\ZepuffTest\1.png)

5. **Open browser and login to Admin UI**
    ```sh
    <Public IP address>:943/admin
    ```

6. **Choose your OpenVPN plan and get activation key**
    ```sh
    <Public IP address>:943/admin
    ```