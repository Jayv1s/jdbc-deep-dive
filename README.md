# jdbc-deep-dive

| **Phase**       | **Goal**                                                          | **Knowledge Involved**                                                                                                                                                            | **Observations**                                                                                                                      |
| --------------- | ----------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| **Phase 1**     | Use and understand **JDBC with H2**                               | - JDBC API (Connection, Statement, ResultSet)<br>- DriverManager<br>- SQL basics (CRUD)<br>- H2 usage                                                                             | ✅ Use Java and H2 embedded DB<br>✅ Focus on using JDBC, not creating it<br>✅ Reuse existing DB tools                                  |
| **Phase 2**     | Build your **own JDBC driver** to talk to a **fake in-memory DB** | - JDBC interfaces (Driver, Connection, Statement, etc.)<br>- Java SPI (Service Provider Interface)<br>- Driver registration with DriverManager<br>- Query parsing & data handling | ✅ You are building the JDBC *provider*, not the *consumer*<br>✅ DB can be just a `Map<String, List<Map<String,Object>>>` for starters |
| **Bonus Phase** | Build your **own micro-database engine** in **C++**               | - File I/O<br>- Indexing (B-Trees, Hash Index)<br>- Query parsing<br>- Transaction basics<br>- Memory management                                                                  | ✅ This is a deep-dive<br>✅ Start with basic insert/select<br>✅ Look at how SQLite works (great reference)                             |


## Phase 1:

---under-construction--