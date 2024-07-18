# Exchange Rate API (FREE)

The **Exchange Rate API** offers real-time and historical exchange rate data for a wide range of currencies. Ideal for developers, financial analysts, and businesses, this API provides accurate and up-to-date information on currency exchange rates, enabling seamless integration into financial applications and services. This API can be found [here](https://rapidapi.com/belchiorarkad-FqvHs2EDOtP/api/mma-api1): 

## Key Features

- **Real-Time Exchange Rates**: Access up-to-the-minute exchange rates for various currency pairs.
- **Historical Data**: Retrieve historical exchange rate data for comprehensive analysis and trend tracking.
- **Currency Conversion**: Easily convert amounts between different currencies using accurate exchange rates.
- **Wide Currency Support**: Covers a vast array of currencies from around the world.

## Getting Started

1. **Sign Up**: Create an account on RapidAPI.
2. **Subscribe**: Select a subscription plan that suits your needs.
3. **API Key**: Obtain your unique API key to begin making requests.
4. **Documentation**: For detailed usage instructions, visit the [MMA API Documentation](https://rapidapi.com/belchiorarkad-FqvHs2EDOtP/api/mma-api1).


## Endpoint: `/exchange-rate`

### Method: GET

### Description:
This endpoint retrieves the exchange rates for all currencies.

### Request:
- No parameters are required.

### Response:
- **Success (200)**: 
  - Returns a JSON object containing the exchange rates for all currencies.
  - Example response:
    ```json
    {
      "USD": 1.0,
      "EUR": 0.85,
      "JPY": 110.53,
      ...
    }
    ```

- **Error (400)**: 
  - Returns a JSON object with an error message if something goes wrong.
  - Example response:
    ```json
    {
      "error": "



## Endpoint: `/exchange-rate/:isoCurrency`

### Method: GET

### Description:
This endpoint retrieves the exchange rate for a specified currency.

### Request:
- **Path Parameter**:
  - `isoCurrency` (string, required): The ISO currency code for which the exchange rate is requested. This parameter is case-insensitive and will be converted to uppercase by the server.

### Response:
- **Success (200)**: 
  - Returns a JSON object containing the exchange rate for the specified currency.
  - Example response:
    ```json
    {
      "currency": "USD",
      "rate": 1.0
    }
    ```

- **Error (400)**: 
  - Returns a JSON object with an error message if something goes wrong.
  - Example response:
    ```json
    {
      "error": "Something went wrong [error message]"
    }
    ```

### Error Handling:
If an error occurs during the request to fetch the exchange rate, the server will log the error message and return a 400 status code with a JSON object containing the error message.

### Example Usage:
```sh
curl -X GET http://yourapi.com/exchange-rate/usd
```
## Commonly Asked Questions

### 1. What kind of data can I access through the Exchange Rate API?
You can access real-time exchange rates, historical data, and currency conversion information for a wide range of currencies.

### 2. How do I authenticate my API requests?
You need to include your API key in the headers of your requests as specified in the API documentation.

### 3. Are there usage limits for the API?
Yes, usage limits depend on the subscription plan you choose. Check the RapidAPI dashboard for specifics.

### 4. Can I access historical exchange rate data?
Yes, the API provides historical exchange rate data, allowing for trend analysis and historical comparisons.

### 5. Is currency conversion supported?
Yes, the API allows for easy currency conversion between different currencies using accurate and up-to-date exchange rates.

For more information and to start using the Exchange Rate API, visit [Exchange Rate API on RapidAPI](https://rapidapi.com/belchiorarkad-FqvHs2EDOtP/api/exchange-rate17).
