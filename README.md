# TRAM v0.1

Threat Report ATT&CK<sup>™</sup> Mapping (TRAM) is a tool to aid analyst in mapping finished reports to ATT&CK. TRAM is currently in its beta phase and is actively being developed.

## Requirements
- [python3](https://www.python.org/) (3.6.1+)
- Google Chrome is our only supported/tested browser

## Installation
Start by cloning this repository.
```
git clone https://github.com/mitre-attack/tram.git
```
From the root of this project, install the PIP requirements.
```
pip install -r requirements.txt
```
If you've never started the project before, you'll need to download the `punkt` and `stopwords` nltk packs before using the application. In a terminal, start a Python REPL and enter the following commands:
```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```

Change server defaults:
``` console
$ python tram.py -H
change default host ('0.0.0.0')
$ python tram.py -P
change default port (9999)
```
Then start the server.
```
python tram.py
```

Once the server has started, point your browser to localhost:9999, and you can then enter a URL on the home page.
It currently takes several minutes to analyze a report, so please do not leave the page while it processes. A pop-up will alert you when the report has been analyzed after being submitted.

## Intended Use
Please note that TRAM is currently intended to be used as a local, single user application. We are aware of the benefit of using the application in a centralized location for multiple analysts to access at once, and will work in the future to add features to make this viable.

## How do I contribute?

We welcome all the help we can get in making TRAM a more useful tool for the community. We have made a working prototype and acknowledge that there will need to be increased efforts in the future to maintain and improve it.

Read [CONTRIBUTING.md](CONTRIBUTING.md) to better understand what we're looking for. There's also a Developer Certificate of Origin that you'll need to sign off on.

## Notice

Copyright 2019 The MITRE Corporation

Approved for Public Release; Distribution Unlimited. Case Number 19-3429.

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

This project makes use of ATT&CK<sup>™</sup>

[ATT&CK Terms of Use](https://attack.mitre.org/resources/terms-of-use/)
