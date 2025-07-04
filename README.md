# cintel-03-reactive
## Project Progress: CC3.2 and CC3.3

### CC3.2: Implement Reactive Calc (Returns Original DataFrame)

- Created a reactive calculation function `filtered_data()` using the `@reactive.calc` decorator.
- For now, `filtered_data()` simply returns the full penguins DataFrame loaded from the `palmerpenguins` package.
- This sets the foundation for reactive data filtering in the app.
- Verified the app runs successfully using this reactive data source.

### CC3.3: Use Filtered Data in Outputs

- Updated all outputs (data tables, data grids, and charts) to use `filtered_data()` instead of directly referencing the original DataFrame.
- Ensured that tables and charts dynamically respond to the reactive data source.
- Confirmed the app runs without errors and displays data correctly.

---


