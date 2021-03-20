# FourSpace

## API Documentation

1. POST "/register"

    Body

    ```
    {
        name
        email
        password
        type ["user","company"]
    }
    ```

2. POST "/login"

    Body

    ```
    {
        email,
        password,
        type ["user","company"]
    }
    ```

    Response

    ```
    {
        token
    }
    ```

3. GET "/profile"

    Body

    ```
    {
        token
    }
    ```

    Response

    ```
    {
        name,
        email,
        available,
        rating
    }
    ```

4. GET "./companies"

    Response

    ```
    {
        companyCount,
        companies[]
    }
    ```
