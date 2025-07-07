# cintel-03-reactive

## Project Progress: CC3.2, CC3.3, and CC3.4

### CC3.2: Implement Reactive Calc (Returns Original DataFrame)

- Created a reactive calculation function `filtered_data()` using the `@reactive.calc` decorator.
- Initially, `filtered_data()` simply returned the full penguins DataFrame loaded from the `palmerpenguins` package.
- This set the foundation for reactive data filtering in the app.
- Verified the app runs successfully using this reactive data source.

### CC3.3: Use Filtered Data in Outputs

- Updated all outputs (data tables, data grids, and charts) to use `filtered_data()` instead of directly referencing the original DataFrame.
- Ensured that tables and charts dynamically respond to the reactive data source.
- Confirmed the app runs without errors and displays data correctly.

### CC3.4: Finalize Reactive Filtering Based on User Input

- Enhanced `filtered_data()` to filter the penguins DataFrame based on species selected in the sidebar checkbox group.
- Implemented `req(input.selected_species_list())` to handle cases where no species are selected and avoid errors.
- Verified that data tables, grids, and all charts update reactively when species selection changes.
- Added sidebar inputs for:
  - Species filter (checkbox group)
  - Attribute selector for visualizations
  - Bin controls for histograms
- Took screenshots demonstrating:
  - The default app state with all species selected
  - The app state after filtering species
- Prepared the app for submission with documented code and screenshots.

---

## How to Run

1. Clone this repository.
2. Install dependencies listed in `requirements.txt`.
3. Run the app using the Shiny Playground or a local environment supporting PyShiny.
4. Use sidebar controls to filter data and explore the penguin dataset interactively.

---

## Files Included

- `app.py`: Main PyShiny app script with reactive filtering and visualizations.
- `requirements.txt`: Python packages required to run the app.
- `.gitignore`: Specifies files and folders to be ignored by Git version control.
- `README.md`: This project overview and documentation file.
- `screenshot1.png`: Screenshot showing the app with default selections and visible code.
- `screenshot2.png`: Screenshot showing the app after changing species filter input.

---

## Live App Link

[Shiny Playground Link Here](https://shinylive.io/py/examples/#code=NobwRAdghgtgpmAXGKAHVA6VBPMAaMAYwHsIAXOcpMAYgAIBBAEyYEszXSoAbOgBWxkAFqToA5YhQDOAHQj0AtEuUrVa5XPoBhNOx6sAXlA6iYxigCcpdVhH6CREDPeGjW1wlClwF3iFPZWADc4RDoYWzooCCY6AFlIqAs4OjYAMzS4ZPIMTToAZVQ4bm5bAHNw8yzrSIFXJzoATWIAV3CWqTJKskIhOmEUqSKS8rpiNLo0lohCE38omLogpNYoACNuOGs4AA8oWe5sXPk6AEkYyjJjTjszMksauzrHZ3OmS+u3aw64WLJiVJwNK2FIkd50DbEQgAa2s0ViMA6XTWoNIAU6l2OeQAYtNZjdZCd1EocXi5nDknQfn8AWULK1UHQwSl-mU4AMLAsEVBoSl2OFiJTklAmOtNly6MkOmK4Md6AB1FLvYEQUFI4gwSZkgn9ITGJnRCGgnibWLcYxZGx2AZM4jvOV0XEzclRSmQmHWcZ0bjEMqsQi6-Wea08vkQVAtMhSPB0IoWNKCzUAd0F0Jj8Ml7JaFjsrTIEajWJOABEgbZRk78Wi8sTawo8qWVSkoFrnTcqQEIBUbcq6LzsCmLEwYwmSsQk78IdhdSkpm3RNB4DHUElLkItlt04sWyQfQ08gAVdetqt2ReDEQtbixd5SQgWVgouhJvVdG1z0+pYhbB3nGex1dyHXbxozoIY4EIVg0mnG1bALaxVV+ScvFdMoWngchrHfbVRCuXkpCLegj1nHC7GBbhLF+AB9UUrgACgASn6UMEIBJI0IwwtD2PD85iNMgJ0oOiIggGMzB2Ji8K2foU1Q9DLlAlsRNYRFNQzcSVPQpYeBaWU8gYCwOIUg07CfVBiACOYeDGTl+0HWJ2PkzCY3NFFTWfdg+hbFcLFgdlLXPQi6GIk8+LWO1p3cK13nISc6JIfx3AochDgAQiYqA0ksf9d1IZw8gAVW8f9kjIbM7DswUaUzMqcyibTuF0yZ6TU0KbiCnQRi7R1SMJRQ6zUPJOt4FtePbNZpw6UZ2AQvzJmIMcJ1iCaAOyAYQIlaJp2SABHFpWGSBzDKcriIAbCDBWMQU+roOtCuKm0AAEwOwGBwt4f5ARIXyKHqsbRCTTz6veb6rosB1S1B-4rFdZtbRmdwUiTKBpy9TwuoqUbSLGOwsfnJw8kVL8IAAcjfbBUH9E1pyTB9fpBy7odAtZI2fFJxmSjsWXXGAixU8yLC6VAfTIQ4MF2VBkikOFrFQHY5DSFqwKEWxIpgAWugYdAY32mNsneCw9bgfYOBCI2doVpWpBViAB1YJg2SjGx1cFLo8wLKjAYd9kjYuCxPftx25H512wON8K6pQqR-EtjUAO4eALCKLt9vmEPBe9YgRSo5O0NsQk5Fz1OpBoiYAF5M+zov88YuQ5DQVAqP2ugK-2rAoDZKi0ka+26LkOgB6pVgMHNbA8yogJ3jWJI+7sQf57bye4GnixZ-n9fB7boQACY+7AfJ7eXpIZDABi8H7jf17buDIwn4oII4Aw4DXy-X5P7xNlmajzAfFmKBP8+c9X4bxPloEQFlmz3F-pGOAACL7APXsAE+axWAlCopsLswgqIwBgAAugyDUHcBonAVAWCcF4JPt3Vg6AsjoMoGUMhuD8D4LAOFJg2BsFeBLmUE+ABdeBwCz4CNftfcMt8IDyQfIQF+CD54n2FpIQ4VEUEQCoiQaYZA4FANkQPE+fARaHDoAACSSr6XymoABC+ctE6PngARgAAzCMvkI7RIjh43zIBPUoBsZG2PfuHQUqiVFqNaOQGxtjdH70CXVExnQzGwDoFYmO+BnEIIAKwxnSQ4mM28nFuJcYAnRoiPa9AgtCcKOwqJ0gZH4nRATP4UCYBPIokEtjoKShEyJJ9sSoOyoUCCrAthdNsUgsAzBihDIoWAAA4pcYgxBplgPzmQXyqA+FFMiWHRpvwy5jImaUWBzCT5zPIAspZNtOhrI2Wk4BthSiqjLgeCwulbnz1ccU4eQhV4fNkW3KAdTZEnPYEYloawRk6O+UCMuJ8hD3FQFIRAAB6JFfphBgowCQGASKKDdx2DEfFSLIKxW4AoBx28FC0SgBC2RVxDLshhWAZR5oIDQhPm8wevyEHEGToynllB2UFIHlyq+w9R7j13OhfwgKN5t3drfKlXdzHP3kfQ1ONFjBQColcDYRyRXuIwPKrxirFZ+T3tXVRiq6T2xPgxW5+rN5ipRhKhaUqpAyvXkagO3syDmoMRwlW8S6SwFtZshBcrIwewUb6gJ6wglUUDaycxoaOUDzbp4IcHqDUZuaeuEUWQ976MUdOfInh7hZGjWEAZbTZCnzDbYr1XtHZ+uLRPMtlho0pqFcAqYaC7zJEoE8l5sDu3vPtQIu1EBJ1yF7N4CwIRV6eJjEamMIEAikAYogARj1hT4hCJinghABG9nIpRZpVLGJbu7fQAAov4bM3MUg-E5B-B+yEuibC8G7VUYFWlDMJK-XadFPEYFfV-Zp4Ea0dM6IxSdb9r2Oj6ZaG0xZNXYmVf0AEpBDG2EII1cEYGmm-sGcM7tpVyqxjVfnUuwALUlyYGkMZkH-18IwO4WwwGxFkFA-fcDLSSMl1KDBhiDF+FnW0TuygBsMAmuVceoElGU62A1VcbVMpL23PI3VU9WRqIXunRJ-WWQZOaqVX5eTEwLUqa1dapgGmyNZm00hw61na7ifnpJv23qg7aN7NGpRiaEkwHs6-XcLcrQFh4zs5pP9HwwLc6-FR1gK4gf8xwkJ6jyAJcvlBOgEBJAQnzlenRSXwuONucCCoFc5YYEC8G4LqbJjOb05qxi9bX47DLrudrl8IBJbLrYX1SWHUb1yhYRlzHhmpNHYPDgos4BlzSHo-1xjTH1bGBMEAu4AC+grX5wcvlpsirAeHucHp56TnbfMKe8HGnMCa1vmJC5fMLKWuNRbfTFqBcWKDZY3qVt7kXbsR2CcpzLvqDsb1y-l5ERXGsA7oHk250cCKJujVmweVLFvNfPa1kb69Ovdfh-nAbWXhs9Y3kIXSE2-1TfHWdgeF3aFNvZBZ2M-q21VCTiLZ7G9KvhZq3eLnGOB46Zc-pinBPGUoLQRghhQhsFMMl-PbAjKqE0P9nLxhNLRsLUFDTgTOv15SFeu9A3NajfzxEAu6zez3609rTGE+7gWVMBuTNgerlihSDLiARrcjWGELoZghX5CkAsKsSUOgAAZehwg6DCRgHa6bWyWHq7jMH+XiuT5hB6aUDXMe499ET8nxr23lezfYJsRlkfeCx5D0saw2J89xkLw3la1aWNgHp4Bxzx3Tv13QOFrWqA6INybqwVdWQF2TrAOX8A55qC7X2skTiBEyA7DIPgIgpBkpb+QCuGIXhC7+sLjwROdG5DW1VizqMV+Ynibn7woAA)

---

## Author

Blessing Aganaga

---


