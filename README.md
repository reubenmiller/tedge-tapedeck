# tedge-flight-recorder
Hackathon topic: record tedge mqtt messages and replay them

## Getting started

**Pre-requisites**

To be able to run this example you need the following:

* [just](https://just.systems/man/en/chapter_5.html)
* docker
* docker compose (v2)

### Starting the device where the recording will be done against

1. Checkout the repository

1. Create a .env file

    ```sh
    touch .env
    ```

    And then add the following content

    ```sh
    DEVICE_ID=myunqiuedeviceid
    ```

2. Start the device demo (where the recorder will be activated on)

    ```sh
    just up-device
    ```

3. Bootstrap the device (so that it can talk with Cumulocity IoT)

    ```sh
    just bootstrap
    ```
