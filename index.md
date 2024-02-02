```python
from main import app

if __name__=='__main__':
    app.run(debug=True)
```


```cpp
template <class Stream>
void handle_request(Stream& stream, http::request<http::string_body>&& request) {
    try {
        // Configura la conexión a la base de datos MySQL
        sql::mysql::MySQL_Driver driver;
        std::unique_ptr<sql::Connection> con(driver.connect("tcp://127.0.0.1:3306", "username", "password"));
        std::unique_ptr<sql::Statement> stmt(con->createStatement());
```
