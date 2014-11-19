
### Regional Biodiversity Implications for Freshwater Fish

{{rg_name}} currently hosts {{baseline_b_fish_count}} freshwater fish species.  [[ hi_{{year}}_b_fish_gain_50th > baseline_b_fish_count / 5 OR hi_{{year}}_b_fish_loss_50th > baseline_b_fish_count / 5]]By {{year}} fish biodiversity in this region is projected to undergo significant change. [[never]]

[[  hi_{{year}}_b_fish_count_90th > baseline_b_fish_count
AND hi_{{year}}_b_fish_count_10th >= baseline_b_fish_count ]]Models agree that regional biodiversity of freshwater fish will increase, by between {{hi_{{year}}_b_fish_count_10th - baseline_b_fish_count}} and {{hi_{{year}}_b_fish_count_90th - baseline_b_fish_count}} species.

[[  hi_{{year}}_b_fish_count_90th > baseline_b_fish_count
AND hi_{{year}}_b_fish_count_10th < baseline_b_fish_count
AND hi_{{year}}_b_fish_count_50th > baseline_b_fish_count
AND hi_{{year}}_b_fish_count_90th - hi_{{year}}_b_fish_count_50th < hi_{{year}}_b_fish_count_50th - baseline_b_fish_count
]]Most models predict an increase in this species count, by up to {{hi_{{year}}_b_fish_count_90th - baseline_b_fish_count, absolute}} species, however some models predict a decrease of as many as {{hi_{{year}}_b_fish_count_10th - baseline_b_fish_count, absolute}} species.

[[  hi_{{year}}_b_fish_count_90th > baseline_b_fish_count
AND hi_{{year}}_b_fish_count_10th < baseline_b_fish_count
AND hi_{{year}}_b_fish_count_90th - hi_{{year}}_b_fish_count_50th >= hi_{{year}}_b_fish_count_50th - baseline_b_fish_count
AND hi_{{year}}_b_fish_count_50th - hi_{{year}}_b_fish_count_10th >= baseline_b_fish_count - hi_{{year}}_b_fish_count_50th
]]There is little agreement between models on whether this species count will increase or decrease. Projections range from a decrease of as many as {{hi_{{year}}_b_fish_count_10th - baseline_b_fish_count, absolute}} species to an increase of up to {{hi_{{year}}_b_fish_count_90th - baseline_b_fish_count, absolute}} species.

[[  hi_{{year}}_b_fish_count_90th > baseline_b_fish_count
AND hi_{{year}}_b_fish_count_10th < baseline_b_fish_count
AND hi_{{year}}_b_fish_count_50th < baseline_b_fish_count
AND hi_{{year}}_b_fish_count_50th - hi_{{year}}_b_fish_count_10th < baseline_b_fish_count - hi_{{year}}_b_fish_count_50th
]]Most models predict a decrease in this species count, by as much as {{hi_{{year}}_b_fish_count_10th - baseline_b_fish_count}}, however some predict an increase of as many as {{hi_{{year}}_b_fish_count_90th - baseline_b_fish_count}} species.

[[  hi_{{year}}_b_fish_count_90th <= baseline_b_fish_count
AND hi_{{year}}_b_fish_count_10th < baseline_b_fish_count
]]Almost all models agree on a decrease in this species count, by between {{hi_{{year}}_b_fish_count_90th - baseline_b_fish_count, absolute}} and {{hi_{{year}}_b_fish_count_10th - baseline_b_fish_count, absolute}}.

[[always]]

[[ hi_{{year}}_b_fish_count_50th =5%= baseline_b_fish_count ]]
Even a relatively stable species count may be the result of gains offset by losses.[[never]]

[[ hi_{{year}}_b_fish_count_50th >5%< baseline_b_fish_count]]
Changes to the region's species count may not be the full story, as gains and losses offset each other.[[never]]

[[ hi_{{year}}_b_fish_loss_90th > 0 ]]
Models agree that by {{year}}, between {{hi_{{year}}_b_fish_loss_90th}} and {{hi_{{year}}_b_fish_loss_10th}} of current fish species will be lost to the region, with a median expected loss of {{hi_{{year}}_b_fish_loss_50th}} species.

[[  hi_{{year}}_b_fish_loss_90th == 0
and hi_{{year}}_b_fish_loss_50th > 0 ]]
Most models project a loss of some species by {{year}}, with a median of {{hi_{{year}}_b_fish_loss_50th}} lost species and some models predicting losses of up to {{hi_{{year}}_b_fish_loss_10th}} species.

[[ hi_{{year}}_b_fish_loss_50th == 0 and hi_{{year}}_b_fish_loss_10th < 0 ]]
Some models project losses of up to {{hi_{{year}}_b_fish_loss_10th}} species, however most models agree that by {{year}} no species will be lost.

[[ hi_{{year}}_b_fish_loss_10th == 0 ]]
Models agree however that by {{year}}, no fish species currently in {{rg_name}} will be lost to the region.

[[always]]

Climate variation in {{rg_name}} may also result in the arrival of species of freshwater fish previously not found in the region.[[never]]

[[ hi_{{year}}_b_fish_gain_10th > 0 ]]
Models agree that by {{year}}, between {{hi_{{year}}_b_fish_gain_10th}} and {{hi_{{year}}_b_fish_gain_90th}} additional fish species will live in the region, with a median expected gain of {{hi_{{year}}_b_fish_gain_50th}} species.

[[  hi_{{year}}_b_fish_gain_10th == 0
and hi_{{year}}_b_fish_gain_50th > 0 ]]
Most models project some fish species arriving by {{year}}, with a median of {{hi_{{year}}_b_fish_gain_50th}} new species and some models predicting up to {{hi_{{year}}_b_fish_gain_90th}} new species.

[[ hi_{{year}}_b_fish_gain_50th == 0 and hi_{{year}}_b_fish_gain_90th < 0 ]]
Some models project gains of up to {{hi_{{year}}_b_fish_gain_90th}} species, however most models agree that by {{year}} no new freshwater fish species will arrive.

[[ hi_{{year}}_b_fish_gain_90th == 0 ]]
However, models agree that by {{year}} no new freshwater fish species will enter the region.

[[ hi_{{year}}_b_fish_gain_90th > 0 ]]

In light of possible species gains, it is important to consider that even Australian natives may behave like invasive pests when entering new space.  Interaction with other species has not been modelled.

[[always]]
