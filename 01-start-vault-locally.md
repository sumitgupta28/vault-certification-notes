# Start Vault Locally

1. Download Vault Binary zip from [Download location](https://www.vaultproject.io/downloads)

2. Unzip the Vault Binary zip

3. Start Valut in Dev mode 

    ```
        vault server -dev
    ```

    **output**

    ```
        You may need to set the following environment variable:

        PowerShell:
        $env:VAULT_ADDR="http://127.0.0.1:8200"
        cmd.exe:
        set VAULT_ADDR=http://127.0.0.1:8200

        The unseal key and root token are displayed below in case you want to
        seal/unseal the Vault or re-authenticate.

        Unseal Key: LcLagQd/e7u2z39MO1eVRJNaJ99ZJBgde299JHcUz0U=
        Root Token: s.ZRPZ5ZTAd4jAAv9Rf1nCaKV5

        Development mode should NOT be used in production installations!

    ```

  AS per above instructions set the VAULT_ADDR enviroment variable depended up on your plateform.  

  **Importent Notes**
   - In dev mode keys/data or any thing you generat are stores in the memory. So in case if you are restarting your vault server you will loose the keys/data. 

   