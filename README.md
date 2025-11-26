<div align="center">

# Mercatto App

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![KivyMD](https://img.shields.io/badge/KivyMD-FFD000?style=for-the-badge&logo=python&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Archived-red?style=for-the-badge)

</div>

A lightweight Point of Sale (POS) and inventory management application built with Python and KivyMD. Mercatto App offers a streamlined solution for small businesses to manage sales, stock, and transactions efficiently.

---

## Legacy Project Context & Security Notice

**Please read before reviewing the code.**

This project is an **experimental artifact** developed when the author was approximately **16 years old**. It represents an initial foray into software development, built in parallel with the learning process of Python and GUI frameworks.

**The author is fully aware of the architectural and security flaws present in this codebase**, specifically:
* **Zero Security / No Backend:** The application connects directly from the client to the MySQL database without an API or middleware layer.
* **Exposed Credentials:** Database credentials and IP addresses are hardcoded within `main.py`.
* **Not Production Ready:** Due to these fundamental design choices made during the learning phase, this application **must not be deployed in a production environment**.

This repository is archived for **historical and educational purposes only**, showcasing the complexity of logic implemented by a beginner with limited prior knowledge.

## Key Features

* **Sales Management:** Process transactions with support for multiple payment methods (Cash, Debit, Credit, Boleto, Cheque).
* **Inventory Control:** Track products, categories, and monitor stock levels in real-time.
* **Sales History:** Comprehensive view of completed sales with detailed records for auditing.
* **Product Catalog:** Quick access to product registry with customizable visibility settings.
* **Discounts & Surcharges:** Apply dynamic adjustments to transactions instantly at checkout.
* **Data Isolation:** Automated database structure creation ensures each user account operates with isolated data.

## Technical Architecture

* **Language:** Python 3.x
* **GUI Core:** Kivy (The underlying graphics engine)
* **UI/Theme Layer:** KivyMD (Material Design component library built on Kivy)
* **Database:** MySQL Server
* **Driver:** mysql-connector-python

## Installation & Setup

### Prerequisites
Ensure you have the following installed on your system:
* Python 3.x
* MySQL Server

### Steps

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/ElyonSantos/Mercatto_app](https://github.com/ElyonSantos/Mercatto_app)
    cd Mercatto_app
    ```

2.  **Install dependencies**
    It is recommended that Kivy and KivyMD be installed explicitly to ensure proper dependency resolution.
    ```bash
    pip install kivy kivymd mysql-connector-python
    ```

3.  **Database Configuration**
    The application is pre-configured to connect to a public test database.

    * **Test User:** `elyon`
    * **Test Password:** `123`

    **Important Note:** Do **not** modify the host settings in `main.py`. The application relies on a specific external MySQL configuration with rudimentary authentication. Changing the host without replicating the complex network and authentication setup locally will result in connection failures. The connection may experience latency due to the public server location, but it is functional for testing purposes.

4.  **Run the application**
    ```bash
    python main.py
    ```

## Usage

1.  **Login:** Use the test credentials (`elyon` / `123`) on the welcome screen.
2.  **Add Products:** Navigate to `Cadastros` -> `Produtos` to register new items in the inventory.
3.  **Make Sales:** Select products from the catalog, apply any necessary discounts or surcharges, choose the payment method, and finalize.
4.  **View Reports:** Access your sales history through the "Consultar vendas" menu.

## Contributing

Since this is an archived legacy project, active maintenance has ceased. However, if you wish to fork it for study:

1.  Fork the project.
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

## License

This project is available for use and modification. See the [LICENSE](LICENSE) file for more details.
