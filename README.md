# Importing Data

The ref_data folder contains csv files to import into the MODELS table. The following commands can be run from your postgres server to easily copy the files in (WIP - to be replaced when Dockerizing, this is not a good long term solution). Obviously, replace with your own username.

\copy wht_ref.models (model_name, game_type_id, unit_size_min, unit_size_max, faction) from '/Users/jaceplute/wht-database/ref_data/kt_ref_data.csv' delimiter ',' CSV HEADER;

\copy wht_ref.models (model_name, game_type_id, unit_size_min, unit_size_max, faction) from '/Users/jaceplute/wht-database/ref_data/aos_ref_data.csv' delimiter ',' CSV HEADER;

\copy wht_ref.models (model_name, game_type_id, unit_size_min, unit_size_max, faction) from '/Users/jaceplute/wht-database/ref_data/40k_ref_data.csv' delimiter ',' CSV HEADER;