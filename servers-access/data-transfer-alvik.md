---
description: >-
  This is a guide on how to transfer data from or to Alvik using the terminal or
  via Filezilla
---

# Data transfer - Alvik

## Using Filezilla

1. **Download** and **install** the [FileZilla client](https://filezilla-project.org) for your OS.
2. Connect to the server with the following settings: \
   **Hostname**: `193.10.16.82`, **port**: `22`, your **username** and **password**. \
   Once connected, you can upload or download files between Alvik and your local machine.

## Using the terminal

1. **Connect** to the server with sftp:

&#x20;`sftp`` `_`username`_`@193.10.16.82` and enter your password when prompted.

2. To **download data** from Alvik to your computer, you can use the following command:

`get -r`` `<mark style="color:green;">`<remote_directory>`</mark>` `<mark style="color:orange;">`<local_directory>`</mark>

3. To **upload data** to Alvik from your computer, you can use the following command:

`put -r`` `<mark style="color:orange;">`<local_directory>`</mark>` `<mark style="color:green;">`<remote_directory>`</mark>
