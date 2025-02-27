
---

### `Part_B\README.md`
```markdown
# Part B: E-commerce - Importance of Redundancy

This directory implements an e-commerce API with a focus on service and data redundancy for reliability and data integrity.

## Objectives
- Learn principles of service and data redundancies.
- Implement an e-commerce API with product, order, and cart management.
- Demonstrate synchronous mirroring and asynchronous replication for high availability and disaster recovery.

## Structure
- **`Basic_Implementation/`**: Base e-commerce API and initial servers.
  - `hello_world.py`: Simple Hello World server (port 3001).
  - `dns_registry.py`: DNS registry server returning server URL (port 3000).
  - `ecommerce_server.py`: Full e-commerce API (port 3001).
  - `database.json`: Primary JSON database.
- **`Synchronous_Mirroring/`**: Synchronous mirroring implementation.
  - `ecommerce_server.py`: API with real-time mirroring to `mirror_database.json`.
  - `database.json`, `mirror_database.json`: Mirrored databases.
- **`Asynchronous_Replication/`**: Asynchronous replication implementation.
  - `ecommerce_server.py`: API with delayed replication to `replica_database.json`.
  - `database.json`, `replica_database.json`: Primary and replicated databases.
- **`frontend/`**: Simple HTML frontend.
  - `index.html`: Interface to view and add products.

## Setup
1. **Install Dependencies**:
   ```bash
   pip install flask
