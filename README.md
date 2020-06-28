# finnhub_ruby

FinnhubRuby - the Ruby gem for the Finnhub API

No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)

This SDK is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.RubyClientCodegen

## Installation

### Build a gem

To build the Ruby code into a gem:

```shell
gem build finnhub_ruby.gemspec
```

Then either install the gem locally:

```shell
gem install ./finnhub_ruby-1.0.0.gem
```

(for development, run `gem install --dev ./finnhub_ruby-1.0.0.gem` to install the development dependencies)

or publish the gem to a gem hosting service, e.g. [RubyGems](https://rubygems.org/).

Finally add this to the Gemfile:

    gem 'finnhub_ruby', '~> 1.0.0'

### Install from Git

If the Ruby gem is hosted at a git repository: https://github.com/GIT_USER_ID/GIT_REPO_ID, then add the following in the Gemfile:

    gem 'finnhub_ruby', :git => 'https://github.com/GIT_USER_ID/GIT_REPO_ID.git'

### Include the Ruby code directly

Include the Ruby code directly using `-I` as follows:

```shell
ruby -Ilib script.rb
```

## Getting Started

Please follow the [installation](#installation) procedure and then run the following code:

```ruby
# Load the gem
require 'finnhub_ruby'

# Setup authorization
FinnhubRuby.configure do |config|
  # Configure API key authorization: api_key
  config.api_key['token'] = 'YOUR API KEY'
  # Uncomment the following line to set a prefix for the API key, e.g. 'Bearer' (defaults to nil)
  #config.api_key_prefix['token'] = 'Bearer'
end

api_instance = FinnhubRuby::DefaultApi.new
symbol = 'symbol_example' # String | symbol
resolution = 'resolution_example' # String | Supported resolution includes <code>1, 5, 15, 30, 60, D, W, M </code>.Some timeframes might not be available depending on the exchange.

begin
  #Aggregate Indicators
  result = api_instance.aggregate_indicator(symbol, resolution)
  p result
rescue FinnhubRuby::ApiError => e
  puts "Exception when calling DefaultApi->aggregate_indicator: #{e}"
end

```

## Documentation for API Endpoints

All URIs are relative to *https://finnhub.io/api/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*FinnhubRuby::DefaultApi* | [**aggregate_indicator**](docs/DefaultApi.md#aggregate_indicator) | **GET** /scan/technical-indicator | Aggregate Indicators
*FinnhubRuby::DefaultApi* | [**company_basic_financials**](docs/DefaultApi.md#company_basic_financials) | **GET** /stock/metric | Basic Financials
*FinnhubRuby::DefaultApi* | [**company_earnings**](docs/DefaultApi.md#company_earnings) | **GET** /stock/earnings | Earnings Surprises
*FinnhubRuby::DefaultApi* | [**company_eps_estimates**](docs/DefaultApi.md#company_eps_estimates) | **GET** /stock/eps-estimate | Earnings Estimates
*FinnhubRuby::DefaultApi* | [**company_executive**](docs/DefaultApi.md#company_executive) | **GET** /stock/executive | Company Executive
*FinnhubRuby::DefaultApi* | [**company_news**](docs/DefaultApi.md#company_news) | **GET** /company-news | Company News
*FinnhubRuby::DefaultApi* | [**company_peers**](docs/DefaultApi.md#company_peers) | **GET** /stock/peers | Peers
*FinnhubRuby::DefaultApi* | [**company_profile**](docs/DefaultApi.md#company_profile) | **GET** /stock/profile | Company Profile
*FinnhubRuby::DefaultApi* | [**company_profile2**](docs/DefaultApi.md#company_profile2) | **GET** /stock/profile2 | Company Profile 2
*FinnhubRuby::DefaultApi* | [**company_revenue_estimates**](docs/DefaultApi.md#company_revenue_estimates) | **GET** /stock/revenue-estimate | Revenue Estimates
*FinnhubRuby::DefaultApi* | [**country**](docs/DefaultApi.md#country) | **GET** /country | Country Metadata
*FinnhubRuby::DefaultApi* | [**covid19**](docs/DefaultApi.md#covid19) | **GET** /covid19/us | COVID-19
*FinnhubRuby::DefaultApi* | [**crypto_candles**](docs/DefaultApi.md#crypto_candles) | **GET** /crypto/candle | Crypto Candles
*FinnhubRuby::DefaultApi* | [**crypto_exchanges**](docs/DefaultApi.md#crypto_exchanges) | **GET** /crypto/exchange | Crypto Exchanges
*FinnhubRuby::DefaultApi* | [**crypto_symbols**](docs/DefaultApi.md#crypto_symbols) | **GET** /crypto/symbol | Crypto Symbol
*FinnhubRuby::DefaultApi* | [**earnings_calendar**](docs/DefaultApi.md#earnings_calendar) | **GET** /calendar/earnings | Earnings Calendar
*FinnhubRuby::DefaultApi* | [**economic_code**](docs/DefaultApi.md#economic_code) | **GET** /economic/code | Economic Code
*FinnhubRuby::DefaultApi* | [**economic_data**](docs/DefaultApi.md#economic_data) | **GET** /economic | Economic Data
*FinnhubRuby::DefaultApi* | [**filings**](docs/DefaultApi.md#filings) | **GET** /stock/filings | Filings
*FinnhubRuby::DefaultApi* | [**financials**](docs/DefaultApi.md#financials) | **GET** /stock/financials | Financial Statements
*FinnhubRuby::DefaultApi* | [**financials_reported**](docs/DefaultApi.md#financials_reported) | **GET** /stock/financials-reported | Financials As Reported
*FinnhubRuby::DefaultApi* | [**forex_candles**](docs/DefaultApi.md#forex_candles) | **GET** /forex/candle | Forex Candles
*FinnhubRuby::DefaultApi* | [**forex_exchanges**](docs/DefaultApi.md#forex_exchanges) | **GET** /forex/exchange | Forex Exchanges
*FinnhubRuby::DefaultApi* | [**forex_rates**](docs/DefaultApi.md#forex_rates) | **GET** /forex/rates | Forex rates
*FinnhubRuby::DefaultApi* | [**forex_symbols**](docs/DefaultApi.md#forex_symbols) | **GET** /forex/symbol | Forex Symbol
*FinnhubRuby::DefaultApi* | [**fund_ownership**](docs/DefaultApi.md#fund_ownership) | **GET** /stock/fund-ownership | Fund Ownership
*FinnhubRuby::DefaultApi* | [**general_news**](docs/DefaultApi.md#general_news) | **GET** /news | General News
*FinnhubRuby::DefaultApi* | [**investors_ownership**](docs/DefaultApi.md#investors_ownership) | **GET** /stock/investor-ownership | Investors Ownership
*FinnhubRuby::DefaultApi* | [**ipo_calendar**](docs/DefaultApi.md#ipo_calendar) | **GET** /calendar/ipo | IPO Calendar
*FinnhubRuby::DefaultApi* | [**major_developments**](docs/DefaultApi.md#major_developments) | **GET** /major-development | Major Developments
*FinnhubRuby::DefaultApi* | [**news_sentiment**](docs/DefaultApi.md#news_sentiment) | **GET** /news-sentiment | News Sentiment
*FinnhubRuby::DefaultApi* | [**pattern_recognition**](docs/DefaultApi.md#pattern_recognition) | **GET** /scan/pattern | Pattern Recognition
*FinnhubRuby::DefaultApi* | [**price_target**](docs/DefaultApi.md#price_target) | **GET** /stock/price-target | Price Target
*FinnhubRuby::DefaultApi* | [**quote**](docs/DefaultApi.md#quote) | **GET** /quote | Quote
*FinnhubRuby::DefaultApi* | [**recommendation_trends**](docs/DefaultApi.md#recommendation_trends) | **GET** /stock/recommendation | Recommendation Trends
*FinnhubRuby::DefaultApi* | [**stock_bidask**](docs/DefaultApi.md#stock_bidask) | **GET** /stock/bidask | Last Bid-Ask
*FinnhubRuby::DefaultApi* | [**stock_candles**](docs/DefaultApi.md#stock_candles) | **GET** /stock/candle | Stock Candles
*FinnhubRuby::DefaultApi* | [**stock_dividends**](docs/DefaultApi.md#stock_dividends) | **GET** /stock/dividend | Dividends
*FinnhubRuby::DefaultApi* | [**stock_splits**](docs/DefaultApi.md#stock_splits) | **GET** /stock/split | Splits
*FinnhubRuby::DefaultApi* | [**stock_symbols**](docs/DefaultApi.md#stock_symbols) | **GET** /stock/symbol | Stock Symbol
*FinnhubRuby::DefaultApi* | [**stock_tick**](docs/DefaultApi.md#stock_tick) | **GET** /stock/tick | Tick Data
*FinnhubRuby::DefaultApi* | [**support_resistance**](docs/DefaultApi.md#support_resistance) | **GET** /scan/support-resistance | Support/Resistance
*FinnhubRuby::DefaultApi* | [**technical_indicator**](docs/DefaultApi.md#technical_indicator) | **POST** /indicator | Technical Indicators
*FinnhubRuby::DefaultApi* | [**transcripts**](docs/DefaultApi.md#transcripts) | **GET** /stock/transcripts | Earnings Call Transcripts
*FinnhubRuby::DefaultApi* | [**transcripts_list**](docs/DefaultApi.md#transcripts_list) | **GET** /stock/transcripts/list | Earnings Call Transcripts List
*FinnhubRuby::DefaultApi* | [**upgrade_downgrade**](docs/DefaultApi.md#upgrade_downgrade) | **GET** /stock/upgrade-downgrade | Stock Upgrade/Downgrade


## Documentation for Models

 - [FinnhubRuby::AggregateIndicators](docs/AggregateIndicators.md)
 - [FinnhubRuby::BasicFinancials](docs/BasicFinancials.md)
 - [FinnhubRuby::Company](docs/Company.md)
 - [FinnhubRuby::CompanyExecutive](docs/CompanyExecutive.md)
 - [FinnhubRuby::CompanyNewsStatistics](docs/CompanyNewsStatistics.md)
 - [FinnhubRuby::CompanyProfile](docs/CompanyProfile.md)
 - [FinnhubRuby::CompanyProfile2](docs/CompanyProfile2.md)
 - [FinnhubRuby::CountryMetadata](docs/CountryMetadata.md)
 - [FinnhubRuby::CovidInfo](docs/CovidInfo.md)
 - [FinnhubRuby::CryptoCandles](docs/CryptoCandles.md)
 - [FinnhubRuby::CryptoSymbol](docs/CryptoSymbol.md)
 - [FinnhubRuby::Development](docs/Development.md)
 - [FinnhubRuby::Dividends](docs/Dividends.md)
 - [FinnhubRuby::EarningEstimate](docs/EarningEstimate.md)
 - [FinnhubRuby::EarningRelease](docs/EarningRelease.md)
 - [FinnhubRuby::EarningResult](docs/EarningResult.md)
 - [FinnhubRuby::EarningsCalendar](docs/EarningsCalendar.md)
 - [FinnhubRuby::EarningsCallTranscripts](docs/EarningsCallTranscripts.md)
 - [FinnhubRuby::EarningsCallTranscriptsList](docs/EarningsCallTranscriptsList.md)
 - [FinnhubRuby::EarningsEstimates](docs/EarningsEstimates.md)
 - [FinnhubRuby::EconomicCalendar](docs/EconomicCalendar.md)
 - [FinnhubRuby::EconomicCode](docs/EconomicCode.md)
 - [FinnhubRuby::EconomicData](docs/EconomicData.md)
 - [FinnhubRuby::EconomicEvent](docs/EconomicEvent.md)
 - [FinnhubRuby::Estimate](docs/Estimate.md)
 - [FinnhubRuby::Filing](docs/Filing.md)
 - [FinnhubRuby::FinancialStatements](docs/FinancialStatements.md)
 - [FinnhubRuby::FinancialsAsReported](docs/FinancialsAsReported.md)
 - [FinnhubRuby::ForexCandles](docs/ForexCandles.md)
 - [FinnhubRuby::ForexSymbol](docs/ForexSymbol.md)
 - [FinnhubRuby::Forexrates](docs/Forexrates.md)
 - [FinnhubRuby::FundOwnership](docs/FundOwnership.md)
 - [FinnhubRuby::IPOCalendar](docs/IPOCalendar.md)
 - [FinnhubRuby::IPOEvent](docs/IPOEvent.md)
 - [FinnhubRuby::Indicator](docs/Indicator.md)
 - [FinnhubRuby::Investor](docs/Investor.md)
 - [FinnhubRuby::InvestorsOwnership](docs/InvestorsOwnership.md)
 - [FinnhubRuby::LastBidAsk](docs/LastBidAsk.md)
 - [FinnhubRuby::MajorDevelopments](docs/MajorDevelopments.md)
 - [FinnhubRuby::News](docs/News.md)
 - [FinnhubRuby::NewsSentiment](docs/NewsSentiment.md)
 - [FinnhubRuby::PatternRecognition](docs/PatternRecognition.md)
 - [FinnhubRuby::PriceTarget](docs/PriceTarget.md)
 - [FinnhubRuby::Quote](docs/Quote.md)
 - [FinnhubRuby::RecommendationTrend](docs/RecommendationTrend.md)
 - [FinnhubRuby::Report](docs/Report.md)
 - [FinnhubRuby::RevenueEstimates](docs/RevenueEstimates.md)
 - [FinnhubRuby::Sentiment](docs/Sentiment.md)
 - [FinnhubRuby::Split](docs/Split.md)
 - [FinnhubRuby::Stock](docs/Stock.md)
 - [FinnhubRuby::StockCandles](docs/StockCandles.md)
 - [FinnhubRuby::StockTranscripts](docs/StockTranscripts.md)
 - [FinnhubRuby::SupportResistance](docs/SupportResistance.md)
 - [FinnhubRuby::TechnicalAnalysis](docs/TechnicalAnalysis.md)
 - [FinnhubRuby::TickData](docs/TickData.md)
 - [FinnhubRuby::TranscriptContent](docs/TranscriptContent.md)
 - [FinnhubRuby::TranscriptParticipant](docs/TranscriptParticipant.md)
 - [FinnhubRuby::Trend](docs/Trend.md)
 - [FinnhubRuby::UpgradeDowngrade](docs/UpgradeDowngrade.md)


## Documentation for Authorization


### api_key


- **Type**: API key
- **API key parameter name**: token
- **Location**: URL query string
