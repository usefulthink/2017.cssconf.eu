# To add / edit speakers

Read the [Content Editing](../README.md#content-editing) section of the README

## Properties

Example

    ---
    speaker_id: lana-del-ray
    talk_id: id-of-the-talk
    name: "Lana Del Ray"
    firstname: "Lana"
    lastname: "Del Rey"
    location: "San Fransisco"
    color: mint
    intro: "Ich bins, Lana Del Ray! Lorem dim sum aluminium dolor sit amit git commit it's lit"
    links:
        - text: "@lanadelrey"
          url: "https://twitter.com/lanadelrey"
        - text: "lanadelrey.com"
          url: "http://lanadelrey.com/"
    ---

    Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy
    voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet
    clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit
    amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam
    nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
    sed diam voluptua. At vero eos et accusam et justo duo dolores et ea
    rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem
    ipsum dolor sit amet.

 - `speaker_id`: unique id for the speaker.
   Will be used in the URL, so it should only contain lowercase-letters
   and dashes. Should also correspond to the filename (in the example that'd be `lana-del-ray.md`)
 - `talk_id`: the id of the talk this speaker will give. Corresponds to a filename (without `.md`-extension) in `../_talks`.
 - `name`: the name of the speaker to be displayed in the header of the site. Is used when either first- or lastname are missing.
 - `firstname`: [optional] The firstname, or the first line of the name for the header of the details-page.
 - `lastname`: [optional] The lastname, or second line of the name for the details-page.
 - `location`: the location (city-name) of the speaker, will be displayed along with the name in teaser and speaker-header.
 - `color`: name of the color (as defined in css) used for both the headline and the background of the teaser-box (see http://2017.cssconf.eu/styleguide/ for the color-names)
 - `intro`: the opening-paragraph for the speaker-page
 - `links`: a sorted list of links to appear below the speaker-description. Each link has to contain the fields `text` and `url`.
 - the content of the document (everything behind the "frontmatter"-/metadata-block – that is, after the `---`) is the content-part of the speaker-details page.
