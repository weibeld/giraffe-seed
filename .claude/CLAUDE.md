# CLAUDE.md — giraffe-seed

This project collects data that is intended to be inserted into the [Giraffe](https://github.com/weibeld/giraffe/) data management platform once it has been created. Details about what Giraffe is can be found in the Giraffe project's [concept doc](https://raw.githubusercontent.com/weibeld/giraffe/refs/heads/main/docs/concept.md)).

## Repository structure

This repository contains a sub-directory for every data set. Data is collected in YAML format (usually a single YAML file per dataset).

## Omission of computed fields

The data files do not include fields that are intended to be implemented as computed fields in Giraffe (that is fields that are automatically determined by Giraffe based on a computation configuration). These intended computed fields are listed in the CLAUDE.md file of the dataset's sub-directory.

## Data conventions

The data files use the following conventions:

- Any field type with a `null` value: "pending", i.e. the value of the field has not yet been determined
- A scalar field with a `"n/a"` value: "not applicable", i.e. the field does not apply to this entry, or the field has no value
- A list field with a `[]` value: "no items", i.e. the list is empty and has no values
