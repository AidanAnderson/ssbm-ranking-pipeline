# ssbm-ranking-pipeline
Automated Super Smash Bros. Melee ranking pipeline

🥇 SSBM Ranking Pipeline

A fully automated Python pipeline for generating competitive Super Smash Bros. Melee player rankings using tournament data from Start.gg.
🎯 Features

    Reads tournament slugs from a file and queries the Start.gg GraphQL API

    Extracts:

        Head-to-head game results

        Set outcomes

        Final placements

    Outputs cleaned CSVs for each tournament

    Computes rankings using:

        TrueSkill (match-based skill with uncertainty modeling)

        Plackett-Luce (placement-based probabilistic ranking)

    Supports incremental data processing, slug tracking, and clear output structure

📂 Output Files (per slug)

    $TourneyName###_games.csv

    $TourneyName###_sets.csv

    $TourneyName###_standings.csv

    trueskill_rankings.csv

    plackett_luce_rankings.csv

🔐 API Key Management

This project uses environment variables to manage your Start.gg API key securely via a .env file and python-dotenv.
