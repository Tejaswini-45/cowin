# CoWin Dashboard

The CoWin Dashboard app displays COVID-19 vaccination data using various charts. It provides an easy-to-understand visualization of vaccination trends, broken down by age and gender, and the overall vaccination progress over the last 7 days.

## Features

- **HTTP GET Request**: When the page is opened, an HTTP GET request is made to the `covidVaccinationDataApiUrl` to fetch the latest vaccination data.
- **Loader Display**: A loader is displayed while the HTTP request is being processed to indicate that the data is being fetched.
- **Data Visualization**: Once the data is successfully fetched, it is displayed using different charts from `recharts`:
  - **Bar Chart**: The vaccination data for the last 7 days is displayed using the `BarChart` component.
  - **Pie Charts**: 
    - Vaccination data by gender is displayed using the `PieChart` component.
    - Vaccination data by age is displayed using another `PieChart` component.
- **Error Handling**: If the HTTP GET request is unsuccessful, a `FailureView` is displayed to inform the user about the failure.




### Running the App
- When the page is opened,
  - An HTTP GET request should be made to **covidVaccinationDataApiUrl**
  - **_loader_** should be displayed while the HTTP request is fetching the data
  - After the data is fetched successfully, the response received should be displayed using different charts from `recharts`
  - The last 7 days vaccination data should be displayed using the `BarChart` component from `recharts`
  - The data for vaccination by gender and vaccination by age should be displayed as two different pie charts using the `PieChart` component from `recharts`
  - If the HTTP GET request made is unsuccessful, then the [FailureView](https://assets.ccbp.in/frontend/react-js/api-failure-view.png) should be displayed

</details>

<details>

<summary>API Requests & Responses</summary>
<br/>


