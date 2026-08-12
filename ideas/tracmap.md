# Devmanic TracMap

## Proposition

**Map the journey. Explore the detail.**

Devmanic TracMap is a reusable interactive schematic mapping component for presenting product journeys, processes and system flows. Selecting a station changes the contextual information panel below or alongside the map.

## Scope

TracMap is the component only. Repository analysis and documentation generation are separate products.

### Semantic vocabulary

- **Lines:** journeys, flows or paths
- **Stations:** stages, components, decisions, controls or events
- **Branches:** exceptional, conditional or alternative paths
- **Feeders:** supporting inputs, systems or dependencies
- **Interchanges:** significant connection or orchestration points
- **Start/end:** journey boundaries
- **Context panel:** details for the selected station

## Component MVP

- original Devmanic visual language;
- configurable lines and stations;
- main, branch, alternative and feeder styles;
- start, normal, interchange and end station types;
- selected-station state;
- dynamic contextual content;
- legend;
- responsive rendering;
- keyboard operation and textual alternative;
- example data and documentation;
- distributable component package.

## Evidence-friendly data model

A station should support:

- title and subtitle;
- summary;
- responsibilities;
- inputs and outputs;
- “So What?” call-out;
- tags and type;
- links;
- optional source evidence;
- related stations;
- accessibility label.

## Excluded scope

- automatic repository analysis;
- AI documentation generation;
- CRA or SBOM claims;
- London Underground/TfL branding or copied map content.

## Future integrations

A semantic TracMap model could later present:

- product journeys;
- data flows;
- security controls;
- deployments;
- vulnerability/incident handling;
- CRA evidence;
- R&D experimentation timelines.

## Naming

Use consistently:

- full: **Devmanic TracMap**
- short: **TracMap**
- code: `TracMap`, `tracMap`, `trac-map`
- preferred package: `@devmanic/tracmap`

A rollback tag must be created before rebranding the existing repository.
