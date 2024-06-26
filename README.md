# Introduction
This is a project generated by [salvo-cli](https://github.com/salvo-rs/salvo-cli). You can run the program and test according to the following commands (for non-sqlite databases, please modify the database connection string first according to the tutorial, and complete the initial work of the data).
😄 The latest version of Salvo requires Rust version 1.75. If your compilation fails, please try upgrading with `rustup update`.
``` shell
//Run the project
cargo run 
//Run tests
cargo test
```
# Project directory description
# SafeWallet
- **Dir:** SafeWallet 
- **Dir:** src         (Source code directory)
    - **Dir:** services         (Module containing business logic services)
        - *File:* user.rs 
        - *File:* mod.rs 
    - *File:* main.rs         (Entry point of application, sets up and starts services)
    - *File:* app_response.rs         (Standardize response)
    - *File:* config.rs         (Module for reading and processing application configuration)
    - **Dir:** routers         (Module containing route handling functions)
        - *File:* mod.rs 
        - *File:* demo.rs 
        - *File:* static_routers.rs 
    - **Dir:** dtos         (Module defining Data Transfer Objects (DTOs) for encapsulating and transporting data)
        - *File:* user.rs 
        - *File:* mod.rs 
    - **Dir:** utils         (Module containing utility functions)
        - *File:* rand_utils.rs 
        - *File:* mod.rs 
    - **Dir:** middleware         (Module containing middleware)
        - *File:* cors.rs 
        - *File:* mod.rs 
        - *File:* handle_404.rs 
        - *File:* jwt.rs 
    - *File:* app_error.rs         (Provides unified error handling functionality)
- **Dir:** assets         (Static resources such as images, JavaScript scripts and CSS style sheets)
    - *File:* favicon.ico 
- **Dir:** config         (Folder containing all configuration files)
    - **Dir:** certs         (Directory for storing certificate files)
        - *File:* key.pem 
        - *File:* cert.pem 
    - *File:* config.yml 
- *File:* Cargo.toml         (Rust project dependency and configuration info)

# About Salvo
You can view the salvo documentation and more examples at https://salvo.rs/ 📖. If our tools have helped you, please star [salvo](https://github.com/salvo-rs/salvo) and [salvo-cli](https://github.com/salvo-rs/salvo-cli), which will greatly encourage us. ❤️