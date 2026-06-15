# Strategy Results Ranking

Zakres: strategie znalezione lokalnie, z pominieciem MMS/Icarus. Ranking sortowany po PF z najlepszego dostepnego podsumowania; dla strategii z OOS uzyto OOS 2025, a dla kandydatow przed OOS uzyto wyniku wewnetrznego 2024.

| Rank | Strategia | Status | PF | Expectancy bps | Trades | Zrodlo | Uwagi |
|---:|---|---|---:|---:|---:|---|---|
| 1 | Daily Compression/Expansion v10 | BLOCKED_BEFORE_OOS | 2,097 | 48,07 | 37 | `data/research/daily_compression_expansion_obgate_v10_final_summary_2024_only.json` | BLOCKED_INTERNAL_VALIDATION_FAIL |
| 2 | Stability First Medium Frequency v11 | V11_BLOCKED_BEFORE_OOS | 1,426 | 18,29 | 87 | `data/research/stability_first_medium_frequency_obgate_v11_final_summary_2024_only.json` | BLOCKED_QUARTER_INSTABILITY |
| 3 | Moderate Range Expansion v12c | V12C_PASS_INTERNAL_GATEKEEPER_READY_FOR_OOS | 1,286 | 16,72 | 126 | `data/research/moderate_range_expansion_obgate_v12c_final_summary_2024_only.json` | Jedyny kandydat z PASS_INTERNAL_GATEKEEPER; OOS 2025 dozwolony. |
| 4 | Portfolio Strategy Factory v12 | V12_BLOCKED_BEFORE_OOS | 1,228 | 12,95 | 152 | `data/research/portfolio_strategy_factory_v12_final_summary_2024_only.json` | BLOCKED_TOP_TRADE_DEPENDENT |
| 5 | HTF Anchored Reaction v6 | V6_RESEARCH_MORE | 1,140 | 6,68 | 82 | `data/research/htf_anchored_reaction_obgate_v6_final_summary.json` | Separacja przetrwala, ale walidacja/coverage/economic nie przeszly. |
| 6 | Daily Regime Continuation v9 | OOS_2025_FAILED | 0,963 | -2,19 | 70 | `data/research/daily_regime_continuation_obgate_v9_final_summary.json` | 2024 kandydat przeszedl selekcje, OOS 2025 ujemny. |
| 7 | Frequent Session Breakout v2 | REJECT_V2_KEEP_FROZEN_V1 | 0,857 | -4,99 | 161 | `data/research/frequent_session_breakout_ob_gate_final_summary.json` | FREQUENT_OOS_FAIL |
| 8 | Alternative OB Validated v5 | V5_REJECT | 0,840 | -7,10 | 184 | `data/research/alternative_obvalidated_v5_final_summary.json` | OOS 2025 ujemny. |
| 9 | HTF Level Acceptance v8 | V8_REJECT | 0,385 | -30,22 | 107 | `data/research/htf_level_acceptance_obgate_v8_final_summary.json` | OOS 2025 zdecydowanie slaby. |
| 10 | Orderbook Scalp v7 | V7_SCALP_NO_PREDICTIVE_EDGE | n/a | n/a | 9307 | `data/research/orderbook_scalp_v7_final_summary.json` | Brak predictive edge; OOS nie uruchomiony. |

## Kod strategii / implementacje

- `src/backtest_ltf_session_breakout_strategy_lab.py` - Session Breakout lab.
- `src/backtest_frequent_session_breakout_grid.py` - Frequent Session Breakout.
- `src/build_orderbook_scalp_events_v7.py` / `src/simulate_orderbook_scalp_events_v7.py` - Orderbook Scalp v7.
- `src/run_ltf_fvg_ifvg_strategy_lab.py` / `src/backtest_ltf_fvg_ifvg_sweep_strategy_grid.py` - LTF FVG/IFVG.
- `src/backtest_ltf_base_strategy_grid.py` - LTF Base Strategy.
- `src/build_daily_regime_continuation_events_v9.py` - Daily Regime Continuation v9.
- `src/build_daily_compression_expansion_events_v10.py` - Daily Compression/Expansion v10.
- `src/build_htf_anchored_reaction_events_v6.py` - HTF Anchored Reaction v6.
- `src/build_htf_level_acceptance_events_v8.py` - HTF Level Acceptance v8.
- `src/build_moderate_range_expansion_v12c_events_2025.py` - Moderate Range Expansion v12c.
- `src/build_alternative_obvalidated_events_v5.py` - Alternative OB Validated v5.
- `src/build_stability_first_medium_frequency_ob_features_v11.py` - Stability First Medium Frequency v11.
- `src/build_portfolio_strategy_factory_events_v12.py` - Portfolio Strategy Factory v12.
- `src/gold_futures/gc_daily_swing_backtester.py` - Gold Futures Daily Swing.
- `mt5/Experts/SessionBreakoutBaselineTester.mq5` and `mt5/Experts/SessionBreakoutBaselineOrderbookGateTester.mq5` - MT5 EAs.
