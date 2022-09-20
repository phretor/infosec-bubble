# Infosec Bubble

News clustering and ranking thing to help infosec bubbles...bubble up!

## Main Idea

- have a well-curated, high-quality list of media outlets
- newsworthy content will be featured by many outlets in the same time interval
- writers use pretty much the same keywords
- popular content will share the same keywords
- popular content will form clusters

## Implementation Roadmap

For each source:

- extract links and words from the title
- extract named entities with SpaCy (for English) and CyNER (for cybersecurity-specific terms)
- assign weights to sources (e.g., links coming from well-known reporters or curated newsletters weight more)
- every hour, cluster stories based on the above features
- represent clusters with the top N named entities extracted from the items

## License

MIT License