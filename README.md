# SpindleNet

    mkdir external
    cd external
    ln -sf /path/to/the/root/of/datasets raw_data
    ln -sf /path/to/the/root/of/caffe-master caffe
    ln -sf /path/to/your/experiments/directory exp
    cd ..
    I haven't get the PSDB datasets yet.So I made some change to format_data.sh and make_datalists.sh.
    format_rawdata.sh, make_datalists.sh and merge_datalists.sh take littel time to run. gen_proposal_datalist.sh runs for about 2 hours. What's more, there are few mistakes in format_rawdata.sh about the root of certain file. 
    
    ./scripts/format_rawdata.sh
    ./scripts/make_datalists.sh
    ./scripts/merge_datalists.sh
    ./scripts/gen_proposal_datalist.sh

    ./scripts/train_base.sh
    
    ./scripts/train_head.sh
    ./scripts/train_body.sh
    ./scripts/train_leg.sh
    ./scripts/train_rarm.sh
    ./scripts/train_larm.sh
    ./scripts/train_rleg.sh
    ./scripts/train_lleg.sh

    ./scripts/train_spindlenet.sh

    ./scripts/test.sh
