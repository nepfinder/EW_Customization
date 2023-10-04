## Frappe CRM App Customization

![269898148-ca9288aa-6937-4e38-a93f-7f584b0aafb3](https://github.com/nepfinder/EW_Customization/assets/64308806/d4c06d02-17ad-4140-acac-404934d7d9c8)



## Installation
1. Install [bench & frappe]([https://frappeframework.com/docs/v14/user/en/installation](https://github.com/nepfinder/CRMCustomization)).

2. Once setup is complete, add the payments app to your bench by running
    ```
    bench get-app https://github.com/nepfinder/ew_customization
    ```
3. Developer Mode
    ```
    $ bench --site <sitename> set-config --global developer_mode 1
    ```
3. Install the payments app on the required site by running
    ```
    bench --site <sitename> install-app ew_customization
    ```
4. Restart Services
     ```
    sudo supervisorctl restart all
    ```


## Update

1. Pull latest code from github
    ```
    cd frappe-bench/apps/ew_customization
    ```   
2. Pull latest version from github
     ```
     git pull
    ```
3. Migrate Site
     ```
    bench --site <sitename> migrate
    ```
4. Restart Services
     ```
    sudo supervisorctl restart all
    ```

#### License

MIT
