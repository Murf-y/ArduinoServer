# Arduino Server

## Description

Simple and fast web server that can be downloaded as an executable and run on any computer without python installed. The server can be used to upload code to an arduino connected to the computer.

## Why?

You can use this server to upload code from a website (POST request) to an arduino connected to a computer. Hence allowing communication between a website and an arduino.

## Usage

1. Download the executable from the releases page
2. Run the executable
3. Send a post request to the server with the code in the body of the request
4. The server will upload the code to the arduino

## How to build the executable

```pyinstaller --onefile --windowed main.py```
This will create an executable in the dist folder
this executable can be run on any computer without python installed

<br>
To run the executable run:
```.\dist\main\main.exe``` in the src directory

## How to run the server, development mode

1. ```pip install -r requirements.txt```
2. ```python main.py```

## Sending a post request

In the post request body, add:

```json
{
    "code": "code here"
}
```

## License

Licensed under the [MIT License](LICENSE)
