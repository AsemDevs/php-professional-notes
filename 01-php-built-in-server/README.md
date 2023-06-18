# PHP Built-in Server

This section provides instructions on how to use PHP's built-in server for local development and testing purposes. The PHP built-in server is not designed for production use.

## Prerequisites

Before getting started, ensure that you have the following prerequisites installed on your system:

- PHP (version 5.4 or later) - You can download and install PHP from the official PHP website ([php.net](https://php.net)).
- Command-line interface (CLI) - You should have access to a command-line interface or terminal.

## Setting up the Built-in Server

Follow these steps to set up and run the PHP built-in server:

1. **Clone or download this repository**: Start by cloning this repository to your local machine or downloading the code as a ZIP file and extracting it.

2. **Navigate to the "PHP Built-in Server" section**: Using the command-line interface, navigate to the "PHP Built-in Server" section of this repository. For example, if you've cloned the repository to your `Documents` folder, use the following command:

   ```shell
   cd ~/Documents/php-professional-notes/PHP-Built-in-Server
   ```

3. **Start the PHP built-in server**: To start the server, run the following command:

   ```shell
   php -S localhost:8000
   ```

   Replace `localhost:8000` with your preferred hostname and port number.

4. **Access your PHP application**: Open your web browser and visit `http://localhost:8000` (or the hostname and port number you specified). You should see your PHP application running.

## Stopping the Server

To stop the PHP built-in server, press `Ctrl + C` in the command-line interface where the server is running. This will gracefully shut down the server.

## Configuration

To override the default document root (i.e. the current directory), use the `-t` flag:

```shell
php -S <host/ip>:<port> -t <directory>
```

If you have a `public/` directory in your project you can serve your project from that directory using the following command:

```shell
php -S localhost:8080 -t public/
```

## Further Reading

For more information about PHP's built-in server, see the [official PHP documentation](https://www.php.net/manual/en/features.commandline.webserver.php).
