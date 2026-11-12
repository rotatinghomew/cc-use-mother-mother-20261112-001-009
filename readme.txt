测试：python3 -m unittest discover -s tests/policy_trials -p 'test_*.py'
构建：python3 -m compileall -q policy_trial_evaluator tests/policy_trials
验收：python3 -m policy_trial_evaluator.review.cli fixtures/demo.json --database /tmp/policy_trial_evaluator-acceptance.sqlite3
所有输入均为本地合成数据，运行不需要网络。
