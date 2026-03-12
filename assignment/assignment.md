# Assignment

## Brief

Write the YML for the following questions.

## Instructions

Paste the answer as YML in the answer code section below each question.

### Question 1

Question: Add 2 more tests each using `dbt_utils` and `dbt-expectations` to `fact_sales`.

Answer:

Specs for `dbt_utils`:

```

- name: bottles_sold
        description: "The number of bottles sold"
        tests:
          - dbt_utils.accepted_range:
              arguments:
                min_value: 0
                max_value: 20000

- name: sale_dollars
        description: "The total sales in dollars"
        tests:
          - dbt_utils.accepted_range:
              arguments:
                min_value: 0
                max_value: 300000

```

Specs for `dbt-expectations`:

```
- name: bottles_sold
        description: "The number of bottles sold"
        tests:
          - dbt_utils.accepted_range:
              arguments:
                min_value: 0
                max_value: 20000

- name: sale_dollars
        description: "The total sales in dollars"
        tests:
          - dbt_utils.accepted_range:
              arguments:
                min_value: 0
                max_value: 300000

```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
