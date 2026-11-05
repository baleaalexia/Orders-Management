# Orders Management

### Manage clients. Organize inventory. Bring orders together.

A Java desktop application that connects client management, product inventory, shopping carts, and billing through a tabbed Swing interface backed by MySQL.

**Java · Swing · MySQL · JDBC · Reflection · Layered Architecture**

---

## Overview

Orders Management follows the workflow from registering a client to building a cart and placing an order. The application stores clients, products, orders, order items, and bills in a relational database, while keeping presentation, business rules, and data access in separate packages.

The desktop window is titled **Agra's** and provides three main sections: **Clients**, **Products**, and **Orders**.

## Features

| Feature | What you can do |
| --- | --- |
| Client management | Add, edit, delete, and search clients by ID. |
| Client validation | Check for an empty client name and validate email format before insertion or updates. |
| Product management | Maintain product names, prices, and stock quantities; search products by ID. |
| Product availability | Select products with stock greater than zero from the ordering dropdown. |
| Shopping cart | Add multiple product entries and clear the current cart. |
| Order processing | Check stock for each cart entry, deduct quantities, and store order items. |
| Billing | Calculate the total and store a bill containing the client, date, and address. |
| Order lookup | Search an order by ID to inspect its client and product entries. |
| Dynamic tables | Generate table columns and rows from model fields using reflection. |
| Persistent storage | Read and write application data through JDBC and MySQL. |

## Technology

- **Java 17+** — a suitable baseline for the records and pattern matching used by the source.
- **Swing and AWT** — desktop interface, tables, dialogs, and event handling.
- **MySQL** — relational data storage.
- **MySQL Connector/J** — JDBC driver; the IntelliJ module references version `8.3.0`.
- **Java Reflection** — generic SQL generation, object mapping, and table generation.
- **Java Streams** — filtering available products and building dropdown values.

The repository includes IntelliJ IDEA module metadata. It does not include a Maven or Gradle build configuration or a bundled JDBC driver.

