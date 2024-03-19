# Spotify Playlist Sorting by Language 

## Overview: This Python script extracts songs from your LIKED playlist on Spotify, fetches their lyrics from Musixmatch, and identifies their dominant language using AWS Comprehend. It then creates new Spotify playlists based on the dominant languages, allowing you to organize your music collection by language. This tool simplifies the process of exploring and enjoying multilingual music content.

## Features

- Automatically fetches liked songs from your Spotify account.
- Extracts lyrics for each song using the Musixmatch API.
- Detects the language of lyrics using AWS Comprehend.
- Creates playlists on Spotify for each detected language.
- Handles rate limiting and API errors robustly.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/giaranjan/spotify_languagesorting.git
```

2. Install required Python packages:

```bash
pip install -r requirements.txt
```

3. Set up Spotify and AWS credentials:

- Obtain Spotify client ID and client secret from the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications).
- Get a Musixmatch API key from [Musixmatch Developer Portal](https://developer.musixmatch.com/).
- Obtain AWS access key ID and secret access key from the [AWS Management Console](https://aws.amazon.com/console/).

4. Update the configuration:

- Replace placeholders in the code with your actual credentials.
- Set the redirect URI in your Spotify Developer Dashboard to `http://localhost:8888/callback`.

## Usage

1. Run the script:

```bash
python Spotify_playlist_sorting.ipynb
```

2. Follow the instructions to authorize the application and retrieve liked songs from Spotify.

3. Sit back and let the script create playlists for your multilingual music collection!

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/improvement`).
3. Make your changes and commit them (`git commit -am 'Add feature/improvement'`).
4. Push to the branch (`git push origin feature/improvement`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Thanks to Spotify, Musixmatch, and AWS for providing APIs and services used in this project.
