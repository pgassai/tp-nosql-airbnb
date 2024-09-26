# Présentation des données

Pour ce TP, nous utiliserons les données AirBnB qui contiennent des informations sur les logements de certaines villes.

| Colonne          | Type   | Description                                    | Exemple                                          |
|------------------|--------|------------------------------------------------|--------------------------------------------------|
| listing_url      | string | URL du logement                                | https://www.airbnb.com/rooms/10091713            |
| name             | string | Nom du logement                                | Surry Hills Studio - Your Perfect Base in Sydney |
| room_type        | string | Type de logement                               | Entire home/apt                                  |
| accommodates     | int    | Nombre de voyageurs                            | 2                                                |
| bedrooms         | int    | Nombre de chambres                             | 1                                                |
| beds             | int    | Nombre de lits                                 | 1                                                |
| amenities        | list   | Liste des équipements dans le logement         | ["TV", "Shampoo", "Washer"]                      |
| price            | float  | Prix pour une nuitée                           | 181.00                                           |
| security_deposit | float  | Dépôt de garantie                              | 300.00                                           |
| cleaning_fee     | flot   | Frais de ménage                                | 50.00                                            |
| extra_people     | float  | Nombre de personnes supplémentaires autorisées | 0.00                                             |
| guests_included  | int    | Nombre de invités inclus                       | 1                                                |
| address          | array  | Adresse du logement                            |                                                  |
| review_scores    | array  | Scores donnés au logement par les visiteurs    |                                                  |
| reviews          | array  | Liste de toutes les notes des voyageurs        |                                                  |

Voici un exemple de données :

```json
{
  "_id": "10233856",
  "listing_url": "https://www.airbnb.com/rooms/10233856",
  "name": "Twin Bed room+MTR Mongkok shopping&My",
  "room_type": "Private room",
  "accommodates": 3,
  "bedrooms": 1,
  "beds": 2,
  "bathrooms": {
    "$numberDecimal": "1.0"
  },
  "amenities": [
    "TV",
    "Wifi",
    "Air conditioning",
    "Doorman",
    "Elevator",
    "Family/kid friendly",
    "Smoke detector",
    "Essentials",
    "Lock on bedroom door",
    "Hangers",
    "Hair dryer"
  ],
  "price": {
    "$numberDecimal": "400.00"
  },
  "extra_people": {
    "$numberDecimal": "0.00"
  },
  "guests_included": {
    "$numberDecimal": "1"
  },
  "address": {
    "street": "Hong Kong, Kowloon, Hong Kong",
    "suburb": "Mong Kok",
    "government_area": "Yau Tsim Mong",
    "market": "Hong Kong",
    "country": "Hong Kong",
    "country_code": "HK",
    "location": {
      "type": "Point",
      "coordinates": [
        114.17073, # longitude
        22.31723 # latitude
      ],
      "is_location_exact": true
    }
  },
  "review_scores": {
    "review_scores_accuracy": 8,
    "review_scores_cleanliness": 9,
    "review_scores_checkin": 9,
    "review_scores_communication": 9,
    "review_scores_location": 10,
    "review_scores_value": 9,
    "review_scores_rating": 83
  },
  "reviews": [
    {
      "_id": "97872534",
      "date": {
        "$date": "2016-08-28T04:00:00Z"
      },
      "reviewer_id": "86705090",
      "reviewer_name": "Shaylyn"
    },
    {
      "_id": "98937596",
      "date": {
        "$date": "2016-09-02T04:00:00Z"
      },
      "reviewer_id": "89941509",
      "reviewer_name": "Mediana Magdalena"
    },
    {
      "_id": "101071855",
      "date": {
        "$date": "2016-09-11T04:00:00Z"
      },
      "reviewer_id": "68236120",
      "reviewer_name": "诗韵"
    },
    {
      "_id": "109671615",
      "date": {
        "$date": "2016-10-22T04:00:00Z"
      },
      "reviewer_id": "45516256",
      "reviewer_name": "Macin"
    },
    {
      "_id": "113172358",
      "date": {
        "$date": "2016-11-10T05:00:00Z"
      },
      "reviewer_id": "15882024",
      "reviewer_name": "Frederick"
    },
    {
      "_id": "122349279",
      "date": {
        "$date": "2016-12-22T05:00:00Z"
      },
      "reviewer_id": "104566474",
      "reviewer_name": "雪霞"
    },
    {
      "_id": "123367430",
      "date": {
        "$date": "2016-12-28T05:00:00Z"
      },
      "reviewer_id": "105204612",
      "reviewer_name": "天玥"
    },
    {
      "_id": "132264707",
      "date": {
        "$date": "2017-02-16T05:00:00Z"
      },
      "reviewer_id": "113134546",
      "reviewer_name": "易菲"
    },
    {
      "_id": "133812078",
      "date": {
        "$date": "2017-02-24T05:00:00Z"
      },
      "reviewer_id": "115757421",
      "reviewer_name": "铖婧"
    },
    {
      "_id": "146465334",
      "date": {
        "$date": "2017-04-23T04:00:00Z"
      },
      "reviewer_id": "107196030",
      "reviewer_name": "小霞"
    },
    {
      "_id": "155314795",
      "date": {
        "$date": "2017-05-28T04:00:00Z"
      },
      "reviewer_id": "132000421",
      "reviewer_name": "菁一"
    },
    {
      "_id": "161164866",
      "date": {
        "$date": "2017-06-17T04:00:00Z"
      },
      "reviewer_id": "16763266",
      "reviewer_name": "Ivan"
    },
    {
      "_id": "165440728",
      "date": {
        "$date": "2017-07-01T04:00:00Z"
      },
      "reviewer_id": "1324465",
      "reviewer_name": "Carol"
    },
    {
      "_id": "175899665",
      "date": {
        "$date": "2017-07-30T04:00:00Z"
      },
      "reviewer_id": "142415535",
      "reviewer_name": "红"
    },
    {
      "_id": "194477007",
      "date": {
        "$date": "2017-09-17T04:00:00Z"
      },
      "reviewer_id": "150440791",
      "reviewer_name": "景鸿"
    },
    {
      "_id": "201751379",
      "date": {
        "$date": "2017-10-09T04:00:00Z"
      },
      "reviewer_id": "57457890",
      "reviewer_name": "Michael"
    },
    {
      "_id": "204822683",
      "date": {
        "$date": "2017-10-20T04:00:00Z"
      },
      "reviewer_id": "69756270",
      "reviewer_name": "Jack"
    },
    {
      "_id": "213590684",
      "date": {
        "$date": "2017-11-22T05:00:00Z"
      },
      "reviewer_id": "157257779",
      "reviewer_name": "Joseph"
    },
    {
      "_id": "214473213",
      "date": {
        "$date": "2017-11-26T05:00:00Z"
      },
      "reviewer_id": "159214167",
      "reviewer_name": "于淼"
    },
    {
      "_id": "219193641",
      "date": {
        "$date": "2017-12-17T05:00:00Z"
      },
      "reviewer_id": "147672503",
      "reviewer_name": "清风"
    },
    {
      "_id": "273083854",
      "date": {
        "$date": "2018-06-05T04:00:00Z"
      },
      "reviewer_id": "8463706",
      "reviewer_name": "Alfred Lord"
    },
    {
      "_id": "289271407",
      "date": {
        "$date": "2018-07-12T04:00:00Z"
      },
      "reviewer_id": "51293354",
      "reviewer_name": "Ize"
    }
  ]
}
```