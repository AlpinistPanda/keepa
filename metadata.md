Fields in PostgreSQL database 

1. **id** (Integer):
    - *Description:* The unique identifier for each book entry.
    - *Example:* `12345`

2. **book_publication_date** (Date):
    - *Description:* The date when the book was published.
    - *Example:* `2020-05-15`

3. **title** (String):
    - *Description:* The title of the book.
    - *Example:* "The Great Gatsby"

4. **isbn** (String):
    - *Description:* The International Standard Book Number (ISBN) of the book in its original format.
    - *Example:* "978-0-7432-7356-5"

5. **isbn13** (String):
    - *Description:* The 13-digit ISBN of the book.
    - *Example:* "9780743273565"

6. **asin** (String):
    - *Description:* The Amazon Standard Identification Number (ASIN) of the book.
    - *Example:* "B00J3EUZOW"

7. **review_count** (Integer):
    - *Description:* The total number of reviews for the book.
    - *Example:* `245`

8. **review_count_dates** (Array of Dates):
    - *Description:* Dates when review counts were recorded.
    - *Example:* `[ "2022-09-15", "2022-09-16", "2022-09-17" ]`

9. **price_dates** (Array of Dates):
    - *Description:* Dates when the price of the book was recorded.
    - *Example:* `[ "2022-09-15", "2022-09-16", "2022-09-17" ]`

10. **price** (Array of Integer):
    - *Description:* Prices of the book corresponding to the recorded dates. It is converted to
    integer by removing the decimals into integer. eg. 799 corresponds to 7.99 in price
    - *Example:* `[ 999, 899, 799 ]`

11. **sales** (Array of Integer):
    - *Description:* The number of sales recorded for the book corresponding to the recorded dates.
    - *Example:* `[ 120, 150, 200 ]`

12. **sales_dates** (Array of Dates):
    - *Description:* Dates when sales data was recorded.
    - *Example:* `[ "2022-09-15", "2022-09-16", "2022-09-17" ]`

13. **sales_ratings** (Array of Decimal):
    - *Description:* Sales ratings of the book corresponding to the recorded dates.
    - *Example:* `[ 4.5, 4.7, 4.9 ]`

14. **sales_ratings_dates** (Array of Dates):
    - *Description:* Dates when sales ratings were recorded.
    - *Example:* `[ "2022-09-15", "2022-09-16", "2022-09-17" ]`

15. **mongodbid** (String):
    - *Description:* The unique identifier in the MongoDB database (if applicable).
    - *Example:* `"60ca3e8a-9e45-45e2-9315-ff3b5cb5567c"`