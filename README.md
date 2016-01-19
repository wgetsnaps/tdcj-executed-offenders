

wget --page-requisites \
     --convert-links \
     --no-host-directories \
     --adjust-extension \
     --output-file /dev/stdout \
     http://www.tdcj.state.tx.us/death_row/dr_executed_offenders.html \
     | tee ./wget.log

wget --convert-links \
     --mirror \
     --adjust-extension \
     --no-parent \
     --no-host-directories \
     --output-file /dev/stdout \
     http://www.tdcj.state.tx.us/death_row/dr_executed_offenders.html \
     | tee ./wget.log     
