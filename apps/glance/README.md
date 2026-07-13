# Glance

[Glance](https://github.com/glanceapp/glance) is self-hosted dashboard. I use it as my firefox home page.

The config is as such:

- [Main file](glance_data/glance.yml) containing 2 pages:
  - Home with basic widgets like calendar RSS feed. There is also 2 custom widgets
    - [Steam top sellers](glance_data/steam-top-sellers.yml)
    - [NPM](glance_data/npm.yml) listing all of my sites.
  - Sport page with various sport results/upcomming matches.
    - [MLB](glance_data/mlb.yml)
    - [NBA](glance_data/nba.yml)
    - [NFL](glance_data/nfl.yml)
    - [NHL](glance_data/nhl.yml)

> [!NOTE]
> I had a yml kind for some reason when I setup Glance so all of the file use the .yml extension instead of .yaml
