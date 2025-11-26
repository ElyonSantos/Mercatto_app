# Mercatto App

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![KivyMD](https://img.shields.io/badge/GUI-KivyMD-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

A lightweight **Point of Sale (POS)** and inventory management application built with **Python** and **KivyMD**. Mercatto App offers a streamlined solution for small businesses to manage sales, stock, and transactions efficiently.

---

## Key Features

* ** Sales Management:** Process transactions seamlessly with support for multiple payment methods (Cash, Debit, Credit, Boleto, Cheque).
* ** Inventory Control:** Track products, categories, and monitor stock levels in real-time.
* ** Sales History:** comprehensive view of completed sales with detailed records for auditing.
* ** Product Catalog:** Quick access to product registry with customizable visibility settings.
* ** Discounts & Surcharges:** Apply dynamic adjustments to transactions instantly at checkout.
* ** Data Isolation:** Automated database structure creation ensures each user account operates with isolated data.

## Tech Stack

* **Language:** Python 3.x
* **GUI Framework:** Kivy and KivyMD
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
    git clone [https://github.com/yourusername/mercatto-app.git](https://github.com/yourusername/mercatto-app.git)
    cd mercatto-app
    ```

2.  **Install dependencies**
    ```bash
    pip install kivy kivymd mysql-connector-python
    ```

3.  **Database Configuration**
    Open `main.py` and configure your MySQL server connection settings (host, user, password).
    > **Note:** It is recommended to use environment variables for sensitive credentials in a production environment.

4.  **Run the application**
    ```bash
    python main.py
    ```

## Usage

1.  **Login:** Enter your credentials on the welcome screen to initialize your session.
2.  **Add Products:** Navigate to `Cadastros` → `Produtos` to register new items in the inventory.
3.  **Make Sales:**
    * Select products from the catalog.
    * Apply any necessary discounts or surcharges.
    * Choose the payment method and finalize.
4.  **View Reports:** Access your sales history through the "Consultar vendas" menu.

## Contributing

Contributions are welcome! Please follow these steps:
1.  Fork the project.
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

Please ensure your changes maintain the existing code structure and include appropriate error handling.

## License

This project is available for use and modification. See the [LICENSE](LICENSE) file for more details.
