# DOCUMENTATION


## Preparation

### Scafold Initial App
The app's intial structure is scaffolded (yeoman) using StongLoop's Loopback API 
framework (The StrongLoop Framework must be installed - preferably Globally: npm install -g strongloop):

```
$ slc loopback

```
### Add Node & Express Intellisense support in VS Code
The primary development tool for this app is Visual Studio Code.  The editor's TypeScript support can be leveraged
to provide Intellisense support when editing Javascript files that reference the Node and Express 
libraries (The TypeScript Definition Manager must be installed - preferably Globally: npm install -g tsd):

```
$ tsd query node express --action install

```
after the install completes, a /typings folder is added to the project root.

## Models

### Mix (Mixes)
```
Title			string	Mix Title [Required]
AudioURL		string	URL to Audio Stream
VideoURL		string	URL to Video Stream
ArtURL			string	URL to Artwork image
DateRecorded	date	Date Recorded
DatePublished	date	Date Published
IsVisible		boolean	Mix Visibility Flag
LengthMinutes	int		Play Length Minutes
LengthSeconds	int		Play Length Seconds
PlayCount		int		Number of Plays
LikeCount		int		Number of "Likes"
Tags			string	Search Tag(s)
```

### Track (Tracks)
```
MixId			int		Related Mix [fk]
Number			int		Track Number [Required]
Title			string	Track Title [Required]
Artist			string	Artist(s)
Year			string	Year
Label			string	Recording Label
ArtURL			string	URL to Track Artwork
IndexMinutes	int		Start Time Minutes
IndexSeconds	int		Start Time Seconds
Release			string	EP/LP Release Name
```
## MongoDB support

### Add LoopBack connector for MongoDB

```
$ npm install loopback-connector-mongodb --save

```
				