tlid-ways
=========

Mapping from TIGER TLIDs to OpenStreetMap ways.

Each file in the [tlid-ways/](tlid-ways) directory contains a list of the TIGER/Line
TLIDs that have ever been referenced by the tags for particular OpenStreetMap ways.
The files are named by county FIPS code (see http://www.itl.nist.gov/fipspubs/fip6-4.htm).
For example, [tlid-ways/06001](06001) is Alameda County, California.

Each file contains a series of lines, each of which contains two numbers. The first is
a TIGER/Line TLID, and the second is an OpenStreetMap way.  For instance,
the Alameda County file begins:

    124992344 11043364
    124992344 6339350
    124992344 7861097
    125010737 27982215

and you can see at http://www.openstreetmap.org/browse/way/11043364 that OSM way 11043364
cites TIGER/Line TLID 124992344 as one of its sources in the tiger:tlid tag.  (The other
three ways of these first four no longer exist.)

Other OSM ways have lost their tiger:tlid tag through editing, so the reason for this
repository is to make it easier to find TLID history that otherwise appears only in
the full OSM history.
