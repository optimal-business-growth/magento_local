# Magento 2 Installation README

This README provides instructions for installing Magento 2 on an Ubuntu 20.04 system. The installation is intended for local development purposes. Please follow the steps below to set up your Magento 2 instance.

## Prerequisites

Before proceeding with the installation, ensure you have the following prerequisites in place:

1. An Ubuntu 20.04 system.
2. Administrative access to the system.


## Installation Steps

### 1. Clone the Repository

You can obtain the installation script provided in this README by cloning the repository containing the script. You can clone the repository using the following command:

```bash
git clone https://github.com/optimal-business-growth/magento_local.git
cd magento_local
```

### 2. Configuration (Optional)

The installation script includes predefined configuration settings. If you wish to customize these settings, edit the script (named `magento.sh`) using a text editor and modify the following variables:

- `BaseUrl`: The base URL for your Magento 2 installation (e.g., `localhost`).
- `DBHost`: The database host (e.g., `localhost`).
- `DBName`: The database name for Magento 2.
- `DBPassword`: The database password.
- `AdminUser`: The Magento admin username.
- `AdminPassword`: The Magento admin password.
- `PublicKey`: The public key for Magento Marketplace.
- `PrivateKey`: The private key for Magento Marketplace.
- `OSUser`: The username of the system user (e.g., `ubuntu`).

You can directly modify the variables in the script.

### 3. Run the Installation Script

Execute the installation script by running the following command:

```bash
bash magento.sh
```

The script will perform the following tasks:

- Update and install Apache.
- Install MySQL and configure the magento user.
- Update and install PHP 7.4 and required modules.
- Install Elasticsearch.
- Install Composer.
- Install Magento.
- Set directory permissions.
- Configure Magento.
- Configure Apache.
- Flush the cache.

The installation process may take some time, so please be patient.

### 4. Access Your Magento 2 Installation

After the script completes successfully, you can access your Magento 2 installation through a web browser. Use the base URL you provided in the configuration step (e.g., `http://localhost`) to access the Magento storefront and admin panel.

## Conclusion

Your Magento 2 installation on Ubuntu 20.04 is now complete. You can start developing and customizing your online store. If you encounter any issues during the installation, please review the script and the configuration settings to ensure they are correctly set.

For further information and guidance on Magento 2, refer to the [official Magento documentation](https://devdocs.magento.com/).

Enjoy your Magento 2 development journey!
