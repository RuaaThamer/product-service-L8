# Best Buy – Product Service

This is the Product Service for the **Best Buy Cloud-Native Final Project**.

The Product Service is a backend REST API responsible for managing the product catalog.
It provides endpoints to retrieve products, retrieve a single product, update products,
and add new products.

The service is implemented in **Rust** and is part of a microservices-based architecture
deployed on **Azure Kubernetes Service (AKS)**.

This project is adapted from the **Algonquin Pet Store (On Steroids)** reference architecture
and rebranded for the Best Buy final project in CST8915.

---

## Architecture Context

The Product Service is consumed by:
- **Store Front** – to display products to customers
- **Store Admin** – to manage product data

In the current implementation, product data is stored in memory.
When the service restarts, the product catalog is reloaded.

---

## Running the Service Locally (Optional)

> ⚠️ Local execution is for development and testing only.  
> In production, this service runs inside Kubernetes (AKS).

### Prerequisites
- Rust toolchain

### Local Development

To run the service locally:

```bash
cargo run